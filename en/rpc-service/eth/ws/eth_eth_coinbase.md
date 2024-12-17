---
title: eth:eth_coinbase - Ethereum
description: Example code for the eth:eth_coinbase ws method. Сomplete guide on how to use eth:eth_coinbase ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
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

