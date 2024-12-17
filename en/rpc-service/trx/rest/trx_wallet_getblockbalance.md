---
title: trx:/wallet/getblockbalance \[POST\] {disallowed}
description: Get all balance change operations in a block.(Note At present, theinterface data can only be queried through the following official nodes47.241.20.47, 161.117.85.97, 161.117.224.116, 161.117.83.38)
---

### Parameters


`hash` - string

`number` - int32

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getblockbalance' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"hash": "0000000001d6f49f02810b1aeb2dab52cbc72bb269388b9cea453a6fd934e7fd"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

