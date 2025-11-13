---
title: Job Booking Status Update
excerpt: >-
  The Status Webhook allows you to receive real-time updates on job booking
  statuses. Whenever a job booking is `booked` or `published`, a Webhook Payload
  will be sent to a URL you define.
deprecated: false
hidden: true
metadata:
  robots: index
---
### Webhook Payload

The following payload will be sent to your configured webhook URL:

```json
{
	"company_id": 123,
	"company_name": "Test GmbH",
	"partner_company_id": "1019261",
	"booking_job_id": 98234,
	"booking_id": 954237,
	"booking_job_title": "Koch (w/m/d)",
	"booking_product_name": "Indeed.com Germany (Sponsored Job)",
	"booking_url": "https://www.indeed.com/koch/",
	"booking_status": "PUBLISHED",
	"transaction_id": "ffdc0e8c-2653-4589-96bb-fef46e9fb520"
}
```

| Field Name             | Type   | Description                                                                                                                   |
| :--------------------- | :----- | :---------------------------------------------------------------------------------------------------------------------------- |
| `company_id`           | int    | The unique Kini ID of the company.                                                                                            |
| `company_name`         | string | The name of the company.                                                                                                      |
| `partner_company_id`   | string | The partner-specific ID of the company, in case it was provided upon company onboarding.                                      |
| `booking_job_id`       | int    | The unique Kini ID of the job for which the job booking was made.                                                             |
| `booking_id`           | int    | The unique Kini ID of the job booking.                                                                                        |
| `booking_job_title`    | string | The title of the job booking.                                                                                                 |
| `booking_product_name` | string | The name of the product which was purchased for this job booking.                                                             |
| `booking_url`          | string | The url of the job booking once it is published. In case of new bookings, this field is empty until the booking is published. |
| `booking_status`       | enum   | The current status of the job booking (`BOOKED`, `PROCESSING`, `PUBLISHED`, `UNPUBLISHED`, `EXPIRED`).                        |
| `transaction_id`       | uuid   | The unique transaction ID associated with the job booking.                                                                    |

<br />

### Status Values

The `status` field can have the following values:

* **BOOKED**: The job booking was successfully created in the database.
* **PROCESSING**: The job booking has been reviewed and is queued to be posted online.
* **PUBLISHED**: The job booking is online on the job board. The `booking_url` field will now be filled.
* **UNPUBLISHED**: The job booking was prematurely taken down by the customer.
* **EXPIRED**: The duration for which the job booking was online has ended. The booking has been removed from the job board.

<br />

### Authentication

Authentication is handled via an API key sent in the request header.

**Example Header**

```text cURL
Authorization: Bearer <API_KEY>
```

The API key can be found in the Kini app, or can be provided to you separately. Ensure that your webhook endpoint is secure and accessible only by authorized requests.

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
* Webhook calls may be retried periodically if no successful response (HTTP 2xx) is received.