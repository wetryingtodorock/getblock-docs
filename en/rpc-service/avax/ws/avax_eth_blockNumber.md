---
title: avax:eth_blockNumber - Avalanche
description: Example code for the avax:eth_blockNumber ws method. Сomplete guide on how to use avax:eth_blockNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_blockNumber",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1d6134e"
}
```

