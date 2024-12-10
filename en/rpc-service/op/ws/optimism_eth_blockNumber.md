---
title: optimism:eth_blockNumber - Optimism
description: Example code for the optimism:eth_blockNumber ws method. Сomplete guide on how to use optimism:eth_blockNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x625581b"
}
```

