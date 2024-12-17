---
title: get_block_count - Monero
description: Example code for the get_block_count json-rpc method. Сomplete guide on how to use get_block_count json-rpc in GetBlock.io Web3 documentation.
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
