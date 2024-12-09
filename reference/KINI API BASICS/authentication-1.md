---
title: Authentication
excerpt: >-
  The Kini API uses **JWT (JSON Web Token)** authentication to ensure secure
  access to the API. This mechanism provides a flexible and secure way to handle
  authentication and eliminates the need for managing passwords directly.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
## Overview

To authenticate with the Kini API:

1. Obtain an **access token** using your username and password from the `/token/`endpoint.
2. Include the access token in the `Authorization` header for all API requests.
3. Refresh the token as needed using the provided `/token/refresh/` endpoint.

***

## Endpoints

### 1. Obtain Token

Use the `POST /token/` endpoint to generate an access and refresh token.

#### Required Request Body:

```json
{
  "username": "your_username",
  "password": "your_password"
}
```

### 3. Request Headers

Once you have an access token, include it in the Authorization header of your API requests:

```
Authorization: Bearer <your_access_token>
```

### 2. Refresh Token

Use the `POST /token/refresh/` endpoint to refresh an expired access token and obtain a new refresh token.

#### Required Request Body:

```json
{
  "refresh": "your_refresh_token"
}
```

#### Example Response:

```json
{
  "access": "new_access_token",
  "refresh": "new_refresh_token"
}
```

***

## Token Validity

* **Access Tokens**: Valid for **5 minutes**. These are used to authenticate API requests.
* **Refresh Tokens**: Valid for **24 hours**. These are used to obtain new access and refresh tokens  without requiring username and password authentication. Each refresh request generates a new refresh token, enhancing security through token rotation.

***

## Best Practices

1. **Store Tokens Securely:**\
   Store tokens in encrypted storage and avoid exposing them in client-side code or log
2. **Use Token Rotation:**\
   Always replace the old refresh token with the new one returned from `/token/refresh/` to minimize security risks.
3. **Handle Token Expiration:**\
   Monitor API responses for expiration errors (HTTP 401) and use the `/token/refresh/` endpoint to refresh tokens before expiration.
4. **Reauthenticate When Necessary:**\
   If both the access and refresh tokens expire, reauthenticate using the `/token/` endpoint with your username and password.
