---
title: trx:/wallet/getnkfromnsk \[POST\] {disallowed}
description: get Nk from Nsk
---

### Parameters


`value` - string, required

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getnkfromnsk' \
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

