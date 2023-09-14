---
title: optimism:rollup_gasPrices \[POST\]
description: Returns the L1 and L2 gas prices that are being used by the Sequencer tocalculate fees.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "rollup_gasPrices",
"params": [],
"id": "getblock.io"}'
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

