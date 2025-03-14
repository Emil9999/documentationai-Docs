---
title: Authentication
excerpt: ''
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

Authentication is now primarily handled through Bearer API Keys. This method simplifies the authentication process and provides more flexible security options.

### Obtaining an API Key

API Keys can be created and managed through the [Kini Partner App](https://app.getkini.com/). When generating a key, you can select your preferred expiration time based on your security requirements.

### Using the API Key

Include your API key in the Authorization header of your requests:

CopyAuthorization: Bearer YOUR\_API\_KEY
Example request using cURL:
bashCopycurl -X GET "[https://api.example.com/resource](https://api.example.com/resource)"
-H "Authorization: Bearer YOUR\_API\_KEY"

```
curl -X GET "https://api.getkini.com/jobs"\
-H "Authorization: Bearer YOUR\_API\_KEY"\
-H "Company-Id: 1"
```

## Legacy Authentication (Deprecated)

The previous authentication flow using username/password credentials to obtain JWT and refresh tokens is still supported but has been deprecated. We recommend migrating to the Bearer API Key authentication method for improved security and simplified integration.

### Username/Password Authentication (Deprecated)

1. Obtain a JWT token by authenticating with username and password
2. Use the refresh token to obtain a new JWT token when needed

These endpoints have been marked as deprecated and may be removed in future versions of the API.