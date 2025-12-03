---
title: Get Job
excerpt: Read a specific Job detail identified by its unique ID.
api:
  file: kini-api.json
  operationId: jobs_retrieve
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---

This endpoint returns a single job belonging to the authenticated company (or the company selected via the `Company-Id` header).

Use the `id` path parameter to look up the job; if the job does not belong to the scoped company, the API responds with a not-found error.

To partially update an existing job, use the `PATCH /jobs/{id}` endpoint, which accepts the same payload shape as job creation.