---
title: web3_clientVersion - Ethereum
description: Example code for the web3_clientVersion ws method. Сomplete guide on how to use web3_clientVersion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "Geth/v1.11.6-stable-ea9e62ca/linux-amd64/go1.20.3"
}
```

