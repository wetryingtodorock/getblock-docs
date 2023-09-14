---
title: trx:/walletsolidity/getblockbynum \[POST\] {disallowed}
description: Queries whether a specified block is confirmed. If the block can beobtained, the block is confirmed by the network if the block cannot beobtained, the block is not confirmed by the network
---

### Parameters


`num` - int32

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/walletsolidity/getblockbynum' \
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

