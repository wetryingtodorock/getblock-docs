---
title: trx:/wallet/getassetissuebyaccount \[POST\] {disallowed}
description: Query the TRC10 token information issued by an account.
---

### Parameters


`address` - string

Address is the Token Issuer account address

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getassetissuebyaccount' \
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

