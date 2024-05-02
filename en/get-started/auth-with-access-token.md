---
lastUpdated: October 24, 2023
title: Authentication with Access Token
description: Get started with GetBlock's APIs by learning how to authenticate your requests with an access token. This beginner-friendly guide provides all the information you need to get your project up and running.
---

# Authentication with Access Token

Once you've created an account and signed in, you'll be directed to the GetBlock Dashboard.

![screenshot 1](https://storage.getblock.io/web/docs/get-started/auth-with-access-token/screenshot_1.webp)

From here, you can set up endpoints to access any supported blockchain. Simply choose a protocol, network, and API interface/add-on.

All endpoints follow the same format:

```https://go.getblock.io/<ACCESS_TOKEN>/```

Note: Ensure you replace <ACCESS_TOKEN> with the specific access token you receive from the GetBlock Dashboard.

To make requests, simply use this full endpoint. Your authorization is achieved through the access token present in the endpoint path. This token also contains essential route information.

Note: Access tokens cannot be sent in headers.

