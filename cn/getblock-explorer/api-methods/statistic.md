---
metaTitle: Method (statistic)
title: statistic \[POST\]
description: Learn how to obtain statistical information from the blockchain using the GetBlock Explorer API. Unlock insights into blockchain data for your applications.
---

### Example

```POST /statistic```

### Request

```
curl --location --request POST 'https://near.getblock.io/explorer/statistic' \
--header 'Content-Type: application/json' \
--header 'Accept: application/json' \
--header 'x-api-key: YOUR-API-KEY' \
--data-raw '{
  "days": 6,
  "type": "tx"
}'
```

### Response

```
[
  {
    "date": "2022-12-07",
    "value": {
      "data": 183813,
      "price": 1.7276842858336163
    }
  }
]
```
