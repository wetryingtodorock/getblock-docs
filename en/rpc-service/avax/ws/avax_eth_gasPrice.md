---
title: avax:eth_gasPrice - Avalanche
description: Example code for the avax:eth_gasPrice ws method. Сomplete guide on how to use avax:eth_gasPrice ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_gasPrice",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5dde50e73"
}
```

