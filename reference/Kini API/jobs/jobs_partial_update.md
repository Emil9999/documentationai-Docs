---
title: Update Job
excerpt: Partially update a Job posting identified by its unique ID.
api:
  file: kini-api.json
  operationId: jobs_partial_update
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---

This endpoint partially updates an existing job belonging to the authenticated company or the company selected via the `Company-Id` header.

The request body accepts the same fields as job creation, but only the provided fields are changed.

If the job does not belong to the scoped company, the API responds with a not-found error.


