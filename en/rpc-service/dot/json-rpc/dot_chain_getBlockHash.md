---
title: dot:chain_getBlockHash \[POST\]
description: Get the block hash for a specific block.
---

### Parameters


`blockNumber` - BlockNumber

number of the block

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "chain_getBlockHash",
"params": ["0x67103a"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x255bc00927df8d33d561792635cbc6bde480a0a505eef5ff28630ece3fc15b32"
}
```

