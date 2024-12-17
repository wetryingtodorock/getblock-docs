---
title: optimism:rollup_gasPrices \[WebSocket\]
description: Returns the L1 and L2 gas prices that are being used by the Sequencer tocalculate fees.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "rollup_gasPrices",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "l1GasPrice": "0x6ed35542d",
        "l2GasPrice": "0xf4240"
    }
}
```

