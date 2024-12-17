---
title: rollup_gasPrices - Optimism
description: Example code for the rollup_gasPrices ws method. Сomplete guide on how to use rollup_gasPrices ws in GetBlock.io Web3 documentation.
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

