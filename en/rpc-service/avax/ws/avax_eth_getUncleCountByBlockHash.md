---
title: avax:eth_getUncleCountByBlockHash - Avalanche
description: Example code for the avax:eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use avax:eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0x3e56c97d34f03b1369c351fa6c9f57c8bfa987c7da40964fab981303e0ef5849"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

