---
title: neo:getbestblockhash \[POST\]
description: Returns the latest block hash of the block chain.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getbestblockhash",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x119a5e29caa2ba8b97d3d0ff4d3e6002a806277d6b873ccc3c84d343f89b095a"
}
```

