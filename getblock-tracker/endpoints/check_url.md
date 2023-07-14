---
title: check_url \[POST\]
description: Check if URL works and get example of the request
---

- https://api.getblock.io/external/webhook/check_url

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

### Body

Object
- **url** _string_ - your target URL to receive webhook notifications.

## Response

### Response successful [200]

String (OK)

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request POST 'https://api.getblock.io/external/webhook/check_url' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '
{
  "url": "https://webhook.site/"
}'
```

Response

```
"OK"
```
