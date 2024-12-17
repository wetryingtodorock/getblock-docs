---
title: trx:/wallet/getReward \[POST\] {disallowed}
description: Get the rewards that a witness or a user has not yet withdrawn.
---

### Parameters


`address` - user's address

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getReward' \
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

