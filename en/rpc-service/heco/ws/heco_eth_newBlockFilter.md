---
title: heco:eth_newBlockFilter - Huobi ECO Chain
description: Example code for the heco:eth_newBlockFilter ws method. Сomplete guide on how to use heco:eth_newBlockFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x8b31f2c2de9ca5c356c17fc495e972da"
}
```

