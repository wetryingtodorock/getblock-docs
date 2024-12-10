---
title: heco:net_peerCount - Huobi ECO Chain
description: Example code for the heco:net_peerCount ws method. Сomplete guide on how to use heco:net_peerCount ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "net_peerCount",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x10"
}
```

