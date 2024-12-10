---
title: bsc:web3_clientVersion - Binance Smart Chain
description: Example code for the bsc:web3_clientVersion ws method. Сomplete guide on how to use bsc:web3_clientVersion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "Geth/v1.2.4-3c5f54fc-20230523/linux-amd64/go1.19.9"
}
```

