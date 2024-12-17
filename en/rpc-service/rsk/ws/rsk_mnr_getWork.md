---
title: rsk:mnr_getWork \[WebSocket\]
description: Returns the hash of the current block, the seedHash, and the boundarycondition to be met (“target”).
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "mnr_getWork",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method mnr_getWork does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

