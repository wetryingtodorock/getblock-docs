---
title: heco:eth_accounts - Huobi ECO Chain
description: Example code for the heco:eth_accounts ws method. Сomplete guide on how to use heco:eth_accounts ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_accounts",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": []
}
```

