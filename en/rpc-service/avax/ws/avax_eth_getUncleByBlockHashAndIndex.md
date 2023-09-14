---
title: avax:eth_getUncleByBlockHashAndIndex \[WebSocket\]
description: Returns information about a uncle of a block by hash and uncle indexposition.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

the uncle’s index position.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0x3e56c97d34f03b1369c351fa6c9f57c8bfa987c7da40964fab981303e0ef5849", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

