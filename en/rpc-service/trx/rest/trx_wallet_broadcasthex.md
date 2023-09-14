---
title: trx:/wallet/broadcasthex \[POST\] {disallowed}
description: Broadcast the protobuf encoded transaction hex string after sign
---

### Parameters


`transaction` - string

Transaction hex after sign

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/broadcasthex' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
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

