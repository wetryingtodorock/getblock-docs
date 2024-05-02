---
metaTitle: Method (tx_list_account)
title: tx_list_account \[POST\]
description: Discover how to retrieve a list of transactions for a specific account using the GetBlock Explorer API. Utilize blockchain data to enhance your applications.
---

### Example

```POST /tx/list/account```

### Request

```
curl --location --request POST 'https://near.getblock.io/explorer/tx/list/account' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--header 'x-api-key: YOUR-API-KEY' \
--data-raw '{
  "account": ,
  "count": 25,
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
