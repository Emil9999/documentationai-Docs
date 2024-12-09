---
title: Getting Started
excerpt: >-
  Welcome to the Kini API! This guide will help you integrate quickly and start
  leveraging our features for managing jobs, candidates, and applications.
deprecated: false
hidden: false
metadata:
  title: ''
  description: ''
  robots: index
next:
  description: ''
---
## Step 1: Authenticate

To interact with the Kini API, you need to authenticate using **JWT (JSON Web Token)**. Follow the steps in the [Authentication Guide](./authentication) to:

1. Obtain an access token using your username and password.
2. Include the token in the `Authorization` header for all API requests.
3. Refresh the token as needed to maintain access.

***

## Step 2: Explore Endpoints

The Kini API provides robust tools for managing jobs, candidates, and applications. Explore the following guides to learn more about specific features:

* [Jobs API](./jobs_list): Manage job postings, including creation, updates, and synchronization.
* [Applications API](./applications_list): Track application statuses and submit new candidates for jobs.

***

## Step 3: Best Practices

Make the most of the Kini API by following these best practices:

* **Secure Tokens**: Keep access and refresh tokens secure. Rotate tokens regularly as described in the [Authentication Guide](./authentication).
* **Use Pagination**: Optimize data handling by enabling pagination. See the [Pagination Guide](./pagination) for details.
* **Handle Errors Gracefully**: Refer to the [Error Handling Guide](./errors) for common scenarios and troubleshooting steps.

***

## Need Help?

If you have questions or need assistance:

* Email us at [support@getkini.com](mailto:support@getkini.com).
* Explore our [Documentation Hub](./) for detailed guides and references.

***

Get started today and streamline your recruitment workflows with the Kini API!
