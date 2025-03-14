---
title: Authentication
excerpt: >-
  The Kini API uses Bearer API Key authentication to ensure secure and
  simplified access to all API resources.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
## Bearer API Key Authentication (Recommended)

This method simplifies authentication and provides more flexible security options.

To authenticate with the Kini API:

1. Obtain an **API Key** in the [Kini Partner App](https://app.getkini.com/).
2. Include the key in the `Authorization` header for all API requests.

***

### 1. Obtaining an API Key

API Keys can be created and managed through the Kini Partner App. When generating a key, you can:

* Select your preferred expiration time based on your security requirements
* Generate multiple keys for different applications or environments
* Revoke keys that are no longer needed

### 3. Using the API Key

Include your API key in the Authorization header of all API requests:

```
Authorization: Bearer <your_access_token>
```

#### Example Request:

```Text cURL
curl --location 'https://api.getkini.com/jobs' 
--header 'Company-Id: 1' \
--header 'Authorization: Bearer YOUR_API_KEY'
```

***

## Best Practices

1. **Key Security:**\
   Store your API key securely and never expose it in client-side code or logs.
2. **Key Rotation:**\
   Rotate your API keys periodically to minimize security risks. Use appropriate expiration times based on your security requirements.

<br />

Note: The legacy JWT authentication method is being phased out. While still supported, we strongly recommend migrating to the Bearer API Key authentication for improved security and ease of use.