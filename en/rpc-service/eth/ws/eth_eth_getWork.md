---
title: eth:eth_getWork \[WebSocket\]
description: Returns the hash of the current block, the seed hash, and the requiredtarget boundary condition.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getWork",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "no mining work available yet"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

