---
title: dash:pruneblockchain \[POST\] {disallowed}
description: Prunes the blockchain up to a specified height or timestamp. The -pruneoption needs to be enabled (disabled by default).
---

### Parameters


`height` - number (int)

The block height to prune up to. May be set to a particular height, or a
unix timestamp to prune blocks whose block time is at least 2 hours
older than the provided timestamp.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "pruneblockchain",
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

