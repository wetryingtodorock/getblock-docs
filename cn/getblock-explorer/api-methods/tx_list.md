---
metaTitle: Method (tx_list)
title: tx_list \[POST\]
description: Access the GetBlock Explorer API to retrieve a list of transactions. Leverage blockchain data for your applications seamlessly and efficiently.
---

### Example

```POST /tx/list```

### Request

```
curl --location --request POST 'https://near.getblock.io/explorer/tx/list' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--header 'x-api-key: YOUR-API-KEY' \
--data-raw '{
  "count": 50,
  "offset": 0
}'
```

### Response

```
[
  {
    "actions": [
      "string"
    ],
    "block_hash": "string",
    "block_height": 0,
    "conversion_fee": "string",
    "created_at": 0,
    "deposit": "string",
    "fee": "string",
    "gas_attached": "string",
    "gas_used": "string",
    "hash": "string",
    "receiver_id": "string",
    "signer_id": "string",
    "successful": true
  }
]
```
