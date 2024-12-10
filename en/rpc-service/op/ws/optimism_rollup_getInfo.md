---
title: optimism:rollup_getInfo - Optimism
description: Example code for the optimism:rollup_getInfo ws method. Сomplete guide on how to use optimism:rollup_getInfo ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rollup_getInfo",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "ethContext": {
            "blockNumber": 17376335,
            "timestamp": 1685506084
        },
        "mode": "verifier",
        "rollupContext": {
            "index": 103110699,
            "queueIndex": 354301,
            "verifiedIndex": 0
        },
        "syncing": false
    }
}
```

