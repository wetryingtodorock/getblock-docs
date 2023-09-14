---
title: trx:/wallet/getincomingviewingkey \[POST\] {disallowed}
description: get incoming viewing key
---

### Parameters


`ak` - string, required

`nk` - string, required

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getincomingviewingkey' \
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

