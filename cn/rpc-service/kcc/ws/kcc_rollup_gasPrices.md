---
title: kcc:rollup_gasPrices \[WebSocket\]
description: Returns the L1 and L2 gas prices that are being used by the Sequencer tocalculate fees.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rollup_gasPrices",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method rollup_gasPrices does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

