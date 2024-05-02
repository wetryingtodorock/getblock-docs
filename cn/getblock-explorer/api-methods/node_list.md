---
metaTitle: Method (block_list)
title: node_list \[POST\]
description: Access the GetBlock Explorer API to retrieve a list of available nodes. Utilize the power of blockchain infrastructure for your applications effortlessly.
---

### Example

```POST /node/list```

### Request

```
curl --location --request POST 'https://near.getblock.io/explorer/node/list' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--header 'x-api-key: YOUR-API-KEY' \
--data-raw '{
  "count": 25,
  "offset": 0,
  "type": "active"
}'
```

### Response

```
[
  {
    "delegators": 596,
    "fee": 0.1,
    "name": "figment.poolv1.near",
    "stake": "32263431092178471868235191059684",
    "status": "active",
    "total": 0.0625
  }
]
```
