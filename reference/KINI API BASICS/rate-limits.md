---
title: Rate Limits
excerpt: Learn about rate limits for the Kini API.
deprecated: false
hidden: false
metadata:
  robots: index
---
Overview

API requests to Kini's API are rate limited to the following per connected company (as identified by the company\_id attached to the request):

* Launch: 60 / minute

For example, if you have 10 customers, the rate limits above would apply to each one separately.

Some endpoints may have different rate limits as specified throughout the API reference.