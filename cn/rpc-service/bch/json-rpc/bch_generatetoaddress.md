---
title: bch:generatetoaddress \[POST\] {disallowed}
description: Mine blocks immediately to a specified address (before the RPC callreturns)
---

### Parameters


`nblocks` - numeric, required

How many blocks are generated immediately.

`address` - string, required

The address to send the newly generated btc to.

`maxtries` - numeric, optional, default=1000000

How many iterations to try.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "generatetoaddress",
"params": [null, null, null],
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

