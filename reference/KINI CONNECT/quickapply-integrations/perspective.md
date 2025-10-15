---
title: Perspective Funnels
excerpt: >-
  This document provides clear instructions on how to configure Perspective so
  that candidate applications are successfully sent to Kini and then forwarded
  to your Applicant Tracking System (ATS) in real time.
deprecated: false
hidden: true
link:
  new_tab: false
metadata:
  robots: index
---
### 🔑 Required Setup in Perspective

To ensure smooth integration, please follow these steps in your Perspective funnel configuration:

#### 1️⃣ Choose your External Job ID method

You must choose exactly one of the following methods to pass the external job ID from your ATS. Do not use both methods.

**Option A: Result page title (recommended) ✨**
Include the external job ID in your final result/thank-you page title by wrapping it in square brackets.

✅ **Example**:
`Thank you – Sales Manager [EU-42]`

In that case _EU-42_ will be used as the external Job ID. Please make sure to not include any spaces inside the brackets.

**Option B: URL parameter utm_term ✨**

If this option is chosen, each application must include the **external job ID** from your ATS as an `utm_term` parameter in the funnel URL.

✅ **Example:**

```
https://your-perspective-page.com/apply?utm_term=123456
```

Here, `123456` is the external job ID that Kini uses to map the application to the correct job. Simply add the parameter when sharing your funnel.

***

#### 2️⃣ Use Perspective Built-in Fields

Perspective’s **built-in candidate fields** (e.g., first name, last name, email) must be used for core candidate data. Supported fields include:

* `firstName`
* `lastName`
* `email`
* `phone`
* `website`
* `address`
* `city`
* `postalCode`
* `country`

These fields are automatically mapped to the candidate profile in Kini and forwarded to the ATS.

***

#### 3️⃣ Fallback Job ID (Optional)

If no `utm_term` is provided (e.g., via a shared application link), candidates will be assigned to a **fallback job** in Kini.

* Share your **fallback job ID** with Kini so we can configure it.

***

#### 4️⃣ Screening Questions

Screening questions must be configured so that their IDs and answer options match your ATS.

* Retrieve the question IDs and options from your ATS (via the Kini API or Job feed).
* In Perspective, add each question using the ID prefixed with `sq_`.

✅ **Example:**
If the ATS question ID is `earliestStartDay`, use `sq_earliestStartDay` in Perspective.
Ensure the **answer choices match 1:1** with those in the ATS.

***

#### :five: File Attachments

Use Perspective's standard file upload field but change the tracking ID to start with **`file_`**:

##### Primary file types (recommended):

* `file_cv` - CV/Resume files
* `file_resume` - Resume files
* `file_cover_letter` - Cover letter files

##### Other file types:

* Any ID with the prefix `file_` also works, i.e `file_certificate`, `file_other` etc.

***

<br />

#### :six: Ignored Fields

Any Perspective field prefixed with **`ignore_`** will be excluded from the synchronization and not forwarded to the ATS.

***

#### :seven: All Other Fields → Comments

Fields that do not match the above criteria will be automatically appended as **comments** to the candidate profile in the ATS.

***

#### :eight: Add Webhook URL

Within your funnel, go to **Apps > Webhooks** and add the provided webhook URL.

`https://api.getkini.com/webhooks/perspective/{company_id}`

* Replace `{company_id}` with the ID of your company in Kini (see [Partner App](https://app.getkini.com/)).
* Add the webhook URL under **Funnel Completed**, not _New Lead_ .
* **Important:** This URL must be added to every funnel for which the integration should be enabled.

<Image align="center" border={false} caption="Make sure to insert the webhook in &#x22;Funnel Completed&#x22;, NOT &#x22;New Lead&#x22;" src="https://files.readme.io/34bb93d113176cf83c7d9c624d690a5bc3e1bb64061765a2be3224e5e3eececb-image.png" />

<br />

### ✅ Summary of Perspective Setup

* [ ] Either embed the **external_id** in brackets in your result page title **or** add **`utm_term`** as a URL parameter to pass the external job ID.
* [ ] Use built-in Perspective fields for candidate basics (name, email, phone, etc.).
* [ ] Provide Kini with a **fallback job ID** (optional but recommended).
* [ ] Use the `file_` prefix in any file upload fields.
* [ ] Configure screening questions using **`sq_<ID>`** and exact answer options.
* [ ] Prefix any non-ATS fields with **`ignore_`** to exclude them.
* [ ] Remaining fields will automatically be stored as comments.
* [ ] Add the **Webhook URL** under Apps > Webhooks for all relevant funnels.

***

### 💬 Need Help?

If you need assistance with the setup or want Kini to review your Perspective funnel, please reach out to us:
📧 **[support@getkini.com](mailto:support@getkini.com)**
