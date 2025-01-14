---
title: Indeed
deprecated: false
hidden: true
metadata:
  robots: index
---
This document provides comprehensive instructions on integrating QuickApply with Indeed. By following these steps, candidate applications submitted through Indeed will be seamlessly forwarded to your customer's Applicant Tracking System (ATS) in real time.

### 📥 How to Generate the Indeed Webhook URL

The webhook URL for Indeed needs to be dynamically generated for each job posting using the following structure:

`https://api.getkini.com/webhooks/indeed/{kini_agency_id}/{kini_company_id}/{external_job_id}`

* **Agency ID**: The unique identifier for the agency Kini. If no agency is involved, use 1 as the default.
* **Company ID**: The unique identifier for the company in Kini.
* **External Job ID**: The unique job identifier provided by the external job platform (e.g., Indeed).

Example:  `https://api.getkini.com/webhooks/indeed/12/345/xyz-67890`

### When to Generate the Webhook URL

The Webhook URL must be generated and included in the XML job feed before the job is submitted to Indeed. Each job posting should have its own unique webhook URL.

### Integrate Webhook URL into Job Feed for Indeed

To ensure that applications from Indeed are correctly routed to the customer’s ATS via the webhook, the `indeed-apply-data` field in the XML job feed must be updated as follows. The webhook URL is inserted into the `indeed-apply-jobUrl`

```xml
<?xml version="1.0" encoding="utf-8"?>
<source>
  <job>
    <title/>
    <date/>
    <referencenumber/>
    <requisitionid/>
    <url/>
    <company/>
    <sourcename/>
    <city/>
    <state/>
    <country/>
    <email/>
    <postalcode/>
    <description/>
    <salary/>
    <education/>
    <jobtype/>
    <category/>
    <experience/>
    <indeed-apply-data>
      <![CDATA
      [indeed-apply-apiToken=1234ABCDE&indeed-apply-jobTitle=
      Professional+Basket+Weaver&indeed-apply-jobId=Sample+ID &indeed-apply-jobCompanyName=My+Favorite+Company
      &indeed-apply-jobLocation=Austin+TX&indeed-apply-jobUrl=
      http%3A%2F%2Fwww.indeed.com&indeed-apply-postUrl=
      https%3A%2F%2Fhookb.in%2FPxOjJqJELNH8lZLZDkpz&indeed-apply-questions
      =https%3A%2F%2Fpastebin.com%2Fraw%2F0vXq9q9b%23]]>
    </indeed-apply-data>
  </job>
</source>
```

For detailed Indeed Documentation, please refer to their: [https://docs.indeed.com/indeed-apply/add-indeed-apply](https://docs.indeed.com/indeed-apply/add-indeed-apply)

We are also happy to support you with your integration efforts, drop us a message at: [support@getkini.com](mailto:support@getkini.com)