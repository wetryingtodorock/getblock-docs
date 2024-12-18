---
title: eth_coinbase - KuCoin Community Chain
description: Example code for the eth_coinbase ws method. Сomplete guide on how to use eth_coinbase ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x7e5f4552091a69125d5dfcb7b8c2659029395bdf"
}
```

