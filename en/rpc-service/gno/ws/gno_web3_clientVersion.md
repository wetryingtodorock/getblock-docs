---
title: gno:web3_clientVersion - Gnosis
description: Example code for the gno:web3_clientVersion ws method. Сomplete guide on how to use gno:web3_clientVersion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "Nethermind/v1.18.2+22c00906/linux-x64/dotnet7.0.5"
}
```

