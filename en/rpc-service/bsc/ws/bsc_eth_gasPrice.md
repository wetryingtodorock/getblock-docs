---
title: bsc:eth_gasPrice \[WebSocket\]
description: Returns a percentile gas unit price for the most recent blocks, in Wei.By default, the last 100 blocks are examined and the 50th percentile gasunit price (that is, the median value) is returned.If there are no blocks, the value for --min-gas-price is returned. Thevalue returned is restricted to values between --min-gas-price and--api-gas-price-max. By default, 1000 Wei and 500GWei.Use the --api-gas-price-blocks, --api-gas-price-percentile , and--api-gas-price-max command line options to configure the eth_gasPricedefault values.
---

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_gasPrice",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xb2d05e00"
}
```

