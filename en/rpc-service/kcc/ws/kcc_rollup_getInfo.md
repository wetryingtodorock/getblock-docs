---
title: kcc:rollup_getInfo - KuCoin Community Chain
description: Example code for the kcc:rollup_getInfo ws method. Сomplete guide on how to use kcc:rollup_getInfo ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rollup_getInfo",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method rollup_getInfo does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

