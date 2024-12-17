---
title: btc:setexcessiveblock \[POST\] {disallowed}
description: Set the excessive block size. Excessive blocks will not be used in theactive chain or relayed.This discourages the propagation of blocks that you consider excessivelylarge.
---

### Parameters


`maxBlockSize` - numeric, required

Excessive block size in bytes. Must be greater than 1000000.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "setexcessiveblock",
"params": [null],
"id": "getblock.io"}'
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

