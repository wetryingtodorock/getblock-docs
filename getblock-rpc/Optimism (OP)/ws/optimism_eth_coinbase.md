---
title: eth_coinbase - Optimism
description: Example code for the eth_coinbase ws method. Сomplete guide on how to use eth_coinbase ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x00000398232e2064f896018496b4b44b3d62751f"
}
```

