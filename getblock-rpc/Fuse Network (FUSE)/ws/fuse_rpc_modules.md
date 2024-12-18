---
title: rpc_modules - Fuse Network
description: Example code for the rpc_modules ws method. Сomplete guide on how to use rpc_modules ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rpc_modules",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "eth": "1.0",
        "net": "1.0",
        "parity": "1.0",
        "rpc": "1.0",
        "secretstore": "1.0",
        "traces": "1.0",
        "web3": "1.0"
    }
}
```

