---
title: heco:eth_blockNumber - Huobi ECO Chain
description: Example code for the heco:eth_blockNumber ws method. Сomplete guide on how to use heco:eth_blockNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x18fd7b4"
}
```

