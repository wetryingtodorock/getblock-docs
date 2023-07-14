---
title: create \[POST\]
description: Create a webhook
---

- https://api.getblock.io/external/webhook/

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

### Body
Object

- **name** _string_ - webhook name.
- **expression** _string_ - boolean expression to trigger the webhook.
- **url** _string_ - your target URL to receive webhook notifications.
- **protocol** _string_ - protocol of the node (BNB Smart chain).
- **network** _string_ - network of the node (mainnet).
- **draft** _bool_ - true, if the webhook is draft, false – if not.
- **enabled** _bool_ - true, if the webhook is enabled, false – if not.

## Response

### Response successful [200]

Array of objects
- **id** _string_ - webhook id.
- **name** _string_ - webhook name.
- **expression** _string_ - boolean expression to trigger the webhook.
- **url** _string_ - your target URL to receive webhook notifications.
- **protocol** _string_ - protocol of the node (BNB Smart chain).
- **network** _string_ - network of the node (mainnet).
- **draft** _bool_ - true, if the webhook is draft, false – if not.
- **enabled** _bool_ - true, if the webhook is enabled, false – if not.
- **failed** _bool_ - true, if URL of the webhook doesn’t work (status code is not 200 or smt).

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request POST 'https://api.getblock.io/external/webhook/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '
{
  "name": "some name",
  "expression": "block_number > 1",
  "url": "https://webhook.site/",
  "network": "mainnet",
  "enabled": true,
  "protocol": "bsc"
}'
```

Response

```
{
    "id": "374173824",
    "name": "some name",
    "expression": "block_number > 1",
    "url": "https://webhook.site/",
    "protocol": "bsc",
    "network": "mainnet",
    "draft": false,
    "enabled": true,
    "failed": false
}
```
