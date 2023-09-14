---
title: zec:generate \[POST\] {disallowed}
description: Mine blocks immediately (before the RPC call returns).Note this function can only be used on the regtest network.
---

### Parameters


`numblocks` - numeric

How many blocks are generated immediately.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "generate",
"params": [2],
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

