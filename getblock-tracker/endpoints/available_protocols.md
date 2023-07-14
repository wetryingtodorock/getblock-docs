---
title: available_protocols \[GET\]
description: Get available protocols
---

- https://api.getblock.io/external/webhook/available_protocols

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

## Response

### Response successful [200]

Array of string

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request GET 'https://api.getblock.io/external/webhook/available_protocols' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

Response

```
["bsc"]
```
