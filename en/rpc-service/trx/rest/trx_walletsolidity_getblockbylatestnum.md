---
title: trx:/walletsolidity/getblockbylatestnum \[POST\] {disallowed}
description: Get last solidity block by number
---

### Parameters


`num` - int32, required

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/walletsolidity/getblockbylatestnum' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"num": 47963997}'
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

