---
title: delete \[DELETE\]
description: Delete a webhook
---

- https://api.getblock.io/external/webhook/{id}

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

### Query params

- **id** _string_ - webhook id.

## Response

### Response is successful [200]

Objects
- **id** _string_ - webhook id.
- **name** _string_ - webhook name.
- **expression** _string_ - boolean expression to trigger the webhook.
- **url** _string_ - your target URL to receive webhook notifications.
- **protocol** _string_ - protocol of the node (BNB Smart chain).
- **network** _string_ - network of the node (mainnet).
- **draft** _bool_ - true, if the webhook is draft, false – if not.
- **enabled** _bool_ - true, if the webhook is enabled, false – if not.
- **failed** _bool_ - true, if URL of the webhook doesn’t work (status code not 200 or smt).

### Response not successful [400, 500]

Object
- **description** _string_ - description of what went wrong.
- **status_code** _int_ - status code of the response.

### Examples

Request

```
curl --location --request DELETE 'https://api.getblock.io/external/webhook/374173824' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

Response

```
{
    "id": "374173824",
    "name": "new some name",
    "expression": "block_number == 1 or block_number == 2",
    "url": "https://webhook.site/",
    "protocol": "bsc",
    "network": "mainnet"
    "draft": false,
    "enabled": true,
    "failed": false
}
```

