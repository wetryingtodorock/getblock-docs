---
title: xmr:get_block_count \[POST\]
description: Look up how many blocks are in the longest chain known to the node.
---

### Parameters

\-

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_block_count",
"params": {},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "count": 2394582,
        "status": "OK",
        "untrusted": false
    }
}
```
