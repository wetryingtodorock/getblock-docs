---
title: trx:/wallet/getzenpaymentaddress \[POST\] {disallowed}
description: get zen payment address
---

### Parameters


`ivk` - string, required

`d` - string, required

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getzenpaymentaddress' \
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

