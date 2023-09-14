---
title: gno:eth_getUncleByBlockHashAndIndex \[WebSocket\]
description: Returns uncle specified by block hash and index.
---

### Parameters


`data` - hex string

32-byte block hash.

`quantity` - hex string

Index of the uncle.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0xc11de1b67dd435ada2b83bbf0bb45cba5efab4e8dd00b100142e799ba902dddc", "0x0"],
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

