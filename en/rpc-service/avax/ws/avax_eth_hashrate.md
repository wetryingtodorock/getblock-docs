---
title: avax:eth_hashrate \[WebSocket\]
description: Returns the number of hashes per second that the node is mining with.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_hashrate",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_hashrate does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

