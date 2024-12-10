---
title: matic:eth_coinbase - Polygon
description: Example code for the matic:eth_coinbase ws method. Сomplete guide on how to use matic:eth_coinbase ws in GetBlock.io Web3 documentation.
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

