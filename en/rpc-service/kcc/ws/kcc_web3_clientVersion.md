---
title: kcc:web3_clientVersion - KuCoin Community Chain
description: Example code for the kcc:web3_clientVersion ws method. Сomplete guide on how to use kcc:web3_clientVersion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "Geth/v1.2.0-stable-555b10c4/linux-amd64/go1.19.3"
}
```

