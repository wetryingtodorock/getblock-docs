---
title: get_all \[GET\]
description: Get all your webhooks
---

- https://api.getblock.io/external/webhook/

## Request

### Headers

- **x-api-key** _string_ - GetBlock API key to access GetBlock Tracker API.

## Response

### Response is successful [200]

Array of objects
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
curl --location --request GET 'https://api.getblock.io/external/webhook/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

Response

```
[
    {
        "id": "374173823",
        "name": "Webhook 1,
        "draft": false,
        "enabled": true
        "failed": false,
        "url": "https://webhook.site/",
        "expression": "(block_number == 1)",
        "protocol": "bsc",
        "network": "mainnet"
    },
    {
        "id": "374173817",
        "name": "Webhook 2",
        "draft": true,
        "enabled": false,
        "failed": true,
        "url": "",
        "expression": "(transaction_transactionHash == "0x91e44d7d3d8ebb0b5a9e4b0a276c0124281750182dfac5abead8efc752e6246a")",
        "protocol": "",
        "network": "
    }
]
```
