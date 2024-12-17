---
title: fuse:eth_coinbase \[WebSocket\]
description: Returns the client coinbase address.
---

### Parameters


\-

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32023,
        "data": "\"\"",
        "message": "No accounts were found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

