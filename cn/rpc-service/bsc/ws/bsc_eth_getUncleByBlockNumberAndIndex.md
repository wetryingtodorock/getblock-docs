---
title: bsc:eth_getUncleByBlockNumberAndIndex \[WebSocket\]
description: Returns uncle specified by block number and index.
---

### Parameters


`quantity|tag` - hex string

Index of the block, or one of the string tags latest, earliest, or
pending, as described in Block Parameter.

`quantity` - hex string

Index of the uncle.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockNumberAndIndex",
"params": ["0x89D2", "0x0"],
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

