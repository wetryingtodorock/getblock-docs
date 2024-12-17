---
title: bsc:eth_newPendingTransactionFilter - Binance Smart Chain
description: Example code for the bsc:eth_newPendingTransactionFilter ws method. Сomplete guide on how to use bsc:eth_newPendingTransactionFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xbb4ee0d0ded95daf7844ea0aae2d1b9f"
}
```

