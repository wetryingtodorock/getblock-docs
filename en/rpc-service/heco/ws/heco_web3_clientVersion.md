---
title: web3_clientVersion - Huobi ECO Chain
description: Example code for the web3_clientVersion ws method. Сomplete guide on how to use web3_clientVersion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "web3_clientVersion",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "Geth/v1.2.2-stable-b07a7152/linux-amd64/go1.19.3"
}
```

