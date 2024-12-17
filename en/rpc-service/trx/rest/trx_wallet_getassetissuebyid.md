---
title: trx:/wallet/getassetissuebyid \[POST\] {disallowed}
description: Query a token by token id. Returns the token object, which contains thetoken name.
---

### Parameters


`value` - int32

The ID of the TRC10 token.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getassetissuebyid' \
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

