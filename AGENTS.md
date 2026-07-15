# AGENTS.md

Notes for AI agents and humans working on this Documentation.AI project. Captured lessons from the migration off ReadMe.io.

## Source layout

```
docs/
  <section>/
    <page>.mdx
  api/
    kini-api.json   # OpenAPI 3.0 spec, imported by documentation.json
documentation.json  # nav, theme, OpenAPI bindings, root config
```

## documentation.json contract (the gotchas)

These all caused 404s or build failures during the migration. Treat as load-bearing:

1. **Paths include the `docs/` prefix.** A file at `docs/kini-api-basics/authentication.mdx` has path `docs/kini-api-basics/authentication`. Paths are relative to the repo root, not the `docs/` directory.

2. **`initialRoute` must point at a path that exists in `navigation.tabs[].groups[].pages[]`.** Otherwise DA returns "This page is not in the navigation. Visitors will see a 404." Add the page to nav before referencing it.

3. **Avoid `index` as a top-level page filename or path.** `docs/index.mdx` is treated specially and does not resolve as a normal page. Use `home.mdx` (or similar) for the landing page and reference it as `docs/home`.

4. **Schema wrapper is required:** `{ "navigation": { "tabs": [...] } }`. Tabs do not live at the root.

5. **Required top-level fields:** `name`, `initialRoute`, `navigation`. Without `initialRoute`, `/` returns 404.

6. **Lucide icon names are kebab-case, no suffix:** `"book-open"`, `"rocket"`, `"webhook"`, `"code"`, `"file-user"`, `"shopping-cart"`. Wrong case fails silently.

7. **OpenAPI per resource group, scoped with `hidden-apis`:**
   ```json
   {
     "group": "Applications",
     "icon": "file-user",
     "openapi": "docs/api/kini-api.json",
     "hidden-apis": ["GET /jobs", "POST /jobs", "GET /companies/", "POST /clickout/"],
     "pages": [{ "title": "Overview", "path": "docs/api/applications/index" }]
   }
   ```
   Without `hidden-apis`, every group with the same `openapi` source renders all endpoints — duplicates everywhere.

## MDX content rules

- **No HTML components.** `<HTMLBlock>`, `<Table>`, `<thead>`, `<tbody>`, `<tr>`, `<td>`, `<th>` are all invalid. Use markdown tables:
  ```
  | Column A | Column B |
  | -------- | -------- |
  | value    | value    |
  ```
- **No HTML entities in double-quoted JSX attributes.** `&#x22;` and `&quot;` decoded inside a `"..."` attribute break syntax. Use single-quoted attributes for any caption/text containing quote characters, e.g. `caption='Use "Funnel Completed", not "New Lead"'`.
- **No external image references to old platforms.** Replace `<Image src="https://files.readme.io/..." />` with a `<Callout>` or local asset.
- **All pages need YAML frontmatter** with `title` and `description`. H1 is auto-generated from `title`; start content at H2.

## Recommended components (from DA Components playbook)

- `<Callout kind="info|tip|alert|danger|success">` for emphasis and warnings
- `<Steps><Step title="..." icon="...">` for procedures
- `<CodeGroup>` for multi-language samples
- `<Request>` / `<Response>` for endpoint examples
- `<ParamField path="..." param-type="..." required="true">` and `<ResponseField name="..." field-type="...">` for API schema docs
- `<Columns cols="2|3|4">` + `<Card title="..." href="..." icon="...">` for landing-page grids
- `<Update label="..." description="..." tags={[]}>` for changelogs
- `<Board><BoardColumn title="..." color="0-8" icon="..."><BoardCard .../></BoardColumn></Board>` for roadmaps
- `<Mermaid>` for sequence/flow diagrams
- `<Tabs><Tab title="..." icon="...">` for platform alternatives

## Subdomain → repo mapping

The link between a `*.documentationai.com` subdomain and a GitHub repo is configured inside the Documentation.AI dashboard (Settings → Integrations → GitHub). GitHub has no knowledge of it. If the dashboard project is recreated, the GitHub App must be re-installed against the target repo.

## Build trigger

Pushes to the connected branch fire the GitHub App webhook and start a build. If a build does not appear to have run, an empty commit (`git commit --allow-empty -m "chore: trigger rebuild"`) re-fires the webhook.

## Source control

- Default branch is `main` on both `Qonexon/kini-api-docs` and `Emil9999/documentationai-Docs`. Both remotes are pushed in sync.
- The historical ReadMe.io source lives on `feature/es/migrate-documentation-ai` of `Qonexon/kini-docs` (PR #1 still open).
