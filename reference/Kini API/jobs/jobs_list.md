---
title: List Jobs
excerpt: Read several Job details identified by their unique Company ID.
api:
  file: kini-api.json
  operationId: jobs_list
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---

This endpoint lists jobs for the authenticated company (or the company selected via the `Company-Id` header).

Results are:

- Paginated using the standard `page` and `page_size` query parameters.
- Searchable via `search`, matching `title`, `location_name`, and `city`.
- Orderable via the `ordering` query parameter, supporting `applied_at`, `created_at`, `updated_at`, and `last_content_update_at`.

Filtering is powered by the Jobs filter set. Common filters include:

- `status` (defaults to only returning active jobs when omitted).
- Location filters such as `city` and `country`.
- `remote`, `import_source`, `external_id`, and timestamp filters such as `created_at`.

For more information on how to combine filters with pagination, see the [Filtering](../filtering.md) section.