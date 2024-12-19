---
title: web3_clientVersion - Rootstock
description: Example code for the web3_clientVersion json-rpc method. Сomplete guide on how to use web3_clientVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "RskJ/4.4.0/Linux/Java1.8/HOP-25b937d"
}
```

