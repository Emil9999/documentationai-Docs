---
title: Create Job
excerpt: Create a Job posting at a Company using the Company's ID.
api:
  file: kini-api.json
  operationId: jobs_create
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---

Jobs are created for the authenticated company or the company selected via the `Company-Id` header.

The API automatically associates the new job with that company and rejects completely empty request bodies.

Use this endpoint to push or sync jobs from ATS or partner systems into Kini.