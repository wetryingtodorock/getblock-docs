---
title: gno:eth_getUncleByBlockNumberAndIndex - Gnosis
description: Example code for the gno:eth_getUncleByBlockNumberAndIndex ws method. Сomplete guide on how to use gno:eth_getUncleByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - hex string

Index of the block, or one of the string tags latest, earliest, or
pending, as described in Block Parameter.

`quantity` - hex string

Index of the uncle.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockNumberAndIndex",
"params": ["0x89D2", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32602,
        "message": "Position Index is incorrect"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

