---
title: trx:/wallet/getexchangebyid \[POST\] {disallowed}
description: Query exchange pair based on id
---

### Parameters


`id` - int32

Transaction pair ID.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getexchangebyid' \
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

