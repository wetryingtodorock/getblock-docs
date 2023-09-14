---
title: kcc:rollup_getInfo \[WebSocket\]
description: Returns useful L2-specific information about the current node.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rollup_getInfo",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method rollup_getInfo does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

