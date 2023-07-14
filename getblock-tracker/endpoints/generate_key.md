---
title: generate_key \[POST\]
description: Generate key to verify sign
---

- https://api.getblock.io/external/webhook/signatory/generate_key

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

## Response

### Response successful [200]

Object
- **key** _string_ - your key.

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request POST 'https://api.getblock.io/external/webhook/signatory/generate_key' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

Response

```
{
  "key": "11k22iia-c45t-404e-9f32-6b5616tt7d793"
}
```
