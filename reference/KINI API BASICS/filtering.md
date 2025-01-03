---
title: Filtering
excerpt: >-
  Efficient data retrieval often requires filtering the dataset to match
  specific criteria. The Kini API supports filtering across multiple endpoints.
deprecated: false
hidden: false
metadata:
  robots: index
---
> ✨ Supported Endpoints
>
> Filtering is supported for the **GET /jobs**, **GET /candidates**, and **GET /applications** endpoints. Ensure you use the correct parameters to avoid unnecessary data processing.

## Filtering Parameters

The following parameters can be used to filter results across different endpoints:

### **GET /jobs**

| Parameter                | Description                                                                            | Filter Type                 | Example Usage                             |
| :----------------------- | :------------------------------------------------------------------------------------- | :-------------------------- | :---------------------------------------- |
| `external_id`            | Filters jobs by their unique external identifier                                       | Exact match                 | `/jobs?external_id=12345`                 |
| `title`                  | Filters jobs by their title                                                            | Contains (case-insensitive) | `/jobs?title=developer`                   |
| `status`                 | Filters jobs by their current status. Possible values: `active`, `deleted`, `archived` | Exact match                 | `/jobs?status=active`                     |
| `remote`                 | Filters jobs by remote work type. Possible values: `remote`, `hybrid`, `on-site`       | Exact match                 | `/jobs?remote=remote`                     |
| `language`               | Filters jobs by the required language                                                  | Exact match                 | `/jobs?language=en`                       |
| `city`                   | Filters jobs by city                                                                   | Contains (case-insensitive) | `/jobs?city=Berlin`                       |
| `country`                | Filters jobs by country                                                                | Exact match                 | `/jobs?country=DE`                        |
| `import_source`          | Filters jobs by the source of their import                                             | Exact match                 | `/jobs?import_source=API`                 |
| `created_at`             | Filters jobs by their creation date                                                    | Greater than or equal       | `/jobs?created_at=2024-01-01`             |
| `updated_at`             | Filters jobs by their last update date                                                 | Greater than or equal       | `/jobs?updated_at=2024-01-01`             |
| `last_content_update_at` | Filters jobs by their last content update date                                         | Greater than or equal       | `/jobs?last_content_update_at=2024-01-01` |

### **GET /applications**

| Parameter                | Description                                                                                                 | Filter Type           | Example Usage                                        |
| :----------------------- | :---------------------------------------------------------------------------------------------------------- | :-------------------- | :--------------------------------------------------- |
| `email`                  | Filters applications by applicant email                                                                     | Exact match           | `/applications?partner_job_id=applicant@example.com` |
| `partner_application_id` | Filters by the partner's application ID                                                                     | Exact match           | `/applications?partner_job_id=8262`                  |
| `partner_job_id`         | Filters by the partner's job ID                                                                             | Exact match           | `/applications?partner_job_id=123_4`                 |
| `partner_company_id`     | Filters by the partner's company ID                                                                         | Exact match           | `/applications?partner=acme-inc`                     |
| `partner`                | Filters by the partner ID                                                                                   | Exact match           | `/applications?partner=4`                            |
| `agency_job_id`          | Filters by the agency's job ID                                                                              | Exact match           | `/applications?agency_job_id=1234`                   |
| `agency`                 | Filters by the agency ID                                                                                    | Exact match           | `/applications?agency=12`                            |
| `channel`                | Filters by the application channel                                                                          | Exact match           | `/applications?channel=LinkedIn`                     |
| `job`                    | Filters by the related job ID                                                                               | Exact match           | `/applications?job=1234`                             |
| `import_source`          | Filters by the source of the application                                                                    | Exact match           | '/applications?import\_source=API'                   |
| `sync_status`            | Filters by the synchronization status. Possible values: `SUCCESS`, `EXPECTED_FAILURE`, `FAILURE`, `NOTSENT` | Exact match           | `/applications?sync_status=SUCCESS`                  |
| `applied_at`             | Filters applications by application date                                                                    | Greater than or equal | `/applications?applied_at=2024-01-01`                |
| `created_at`             | Filters applications by their creation date                                                                 | Greater than or equal | `/applications?created_at=2024-01-01`                |
| `updated_at`             | Filters applications by their last update date                                                              | Greater than or equal | `/applications?updated_at=2024-01-01`                |

### **GET /companies**

| Parameter               | Description                                                            | Filter Type                 | Example Usage                           |
| :---------------------- | :--------------------------------------------------------------------- | :-------------------------- | :-------------------------------------- |
| `name`                  | Filters companies by their name                                        | Contains (case-insensitive) | `/companies?name=Acme`                  |
| `ats`                   | Filters companies by their applicant tracking system (ATS)             | Exact match                 | `/companies?ats=personio`               |
| `candidate_sync_active` | Filters companies by candidate synchronization status (`true`/`false`) | Exact match                 | `/companies?candidate_sync_active=true` |
| `job_sync_active`       | Filters companies by job synchronization status (`true`/`false`)       | Exact match                 | `/companies?job_sync_active=false`      |

## Example Requests

1. **Filter Jobs by Status and Location**\
   Retrieve all active jobs located in Berlin:
   ```
   GET /jobs?status=active&location=Berlin
   ```
2. **Filter Candidates by Creation Date**\
   Retrieve candidates created after January 1, 2024:
   ```text
   GET /candidates?created_at=2024-01-01
   ```

## Response Format

Filtered requests return the same response format as paginated requests, with metadata fields like count, next, and previous. The results array will contain only entries matching the specified filters.

### Example Response

```json
{
  "count": 125,
  "next": "https://api.getkini.com/jobs?status=active&page=1&limit=20",
  "previous": null,
  "results": [
    {
      "id": 42,
      "title": "Software Developer",
      "status": "active"
    },
    {
      "id": 43,
      "title": "Data Scientist",
      "status": "active"
    }
  ]
}
```

## Best Practices

1. **Combine Filtering with Pagination**\
   Use filters together with pagination to efficiently navigate large datasets while retrieving only relevant data.

   Example:

   ```text
   GET /jobs?status=active&location=Berlin&page=1&limit=20
   ```
2. **Validate Filter Parameters**\
   Ensure your filter parameters are valid for the specified endpoint. Invalid filters will be ignored by the API.
3. **Use Date Filters Wisely**\
   When using date filters like `created_at`, ensure you format the date correctly to avoid errors.