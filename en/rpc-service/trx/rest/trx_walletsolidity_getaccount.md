---
title: trx:/walletsolidity/getaccount \[POST\] {disallowed}
description: get solidity account
---

### Parameters


`address` - string, required

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/walletsolidity/getaccount' \
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

