---
title: Job Booking Status Update
excerpt: >-
  The Job Booking Status Webhook allows you to receive real-time updates on
  application statuses. Whenever a status update occurs, a Webhook Payload will
  be sent to a URL you define.
deprecated: false
hidden: false
metadata:
  robots: index
---
### Webhook Payload

The following payload will be sent to your configured webhook URL:

```json
{
    "company_id": 123,
    "partner_id": 10,
    "application_id": 45213,
  	"partner_company_id":"1019261",
    "partner_application_id": "123",
    "external_job_id": "1604531",
    "status": "SUCCESS",
    "failure_error": null
}
```

| Field Name               | Type   | Description                                                                                                 |
| :----------------------- | :----- | :---------------------------------------------------------------------------------------------------------- |
| `company_id`             | int    | The unique Kini ID of the company.                                                                          |
| `partner_id`             | int    | The unique Kini ID of the partner.                                                                          |
| `application_id`         | int    | The unique Kini ID of the application.                                                                      |
| `partner_company_id`     | string | The partner-specific ID of the company, in case it was provided upon company onboarding.                    |
| `partner_application_id` | string | The partner-specific ID of the application, in case it was provided upon application creation.              |
| `external_job_id`        | string | The external job ID.                                                                                        |
| `status`                 | enum   | The current synchronization status of the application (`SUCCESS`, `FAILURE`, `EXPECTED_FAILURE`, `NOTSENT`) |
| `failure_error`          | string | Error details if the synchronization failed (otherwise `null`).                                             |

<br />

### Status Values

The `status` field can have the following values:

* **SUCCESS**: The application was synchronized successfully.
* **FAILURE**: An error occurred during synchronization. Failure details are provided in the field `failure_error`.
* **NOTSENT**: Synchronization hasn't been set to the ATS or is still in progress.
* **EXPECTED\_FAILURE**: Synchronization failed due to an expected error, such as `DuplicateApplicationError`, `JobNotPublishedError`

<br />

### Authentication

Authentication is handled via an API key sent in the request header.

**Example Header**

```text cURL
Authorization: Bearer <API_KEY>
```

The API key will be provided to you separately. Ensure that your webhook endpoint is secure and accessible only by authorized requests.

<br />

### Setting Up Your Webhook URL

Please provide us with your desired Webhook URL so we can configure it in our system.

**Example URL**

```text
https://your-domain.com/kini-status
```

<br />

### Notes

* Ensure your webhook URL supports HTTPS for secure communication.
* Implement robust handling for the webhook payload, especially for the `failure_error` field.
* Webhook calls may be retried periodically if no successful response (HTTP 2xx) is received.