---
title: matic:eth_coinbase \[WebSocket\]
description: Returns the client coinbase address.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "code": -32000,
        "message": "etherbase must be explicitly specified"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

