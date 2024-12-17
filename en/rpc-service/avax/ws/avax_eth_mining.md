---
title: avax:eth_mining \[WebSocket\]
description: Returns true if client is actively mining new blocks.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_mining",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_mining does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

