---
title: eth_newPendingTransactionFilter - Huobi ECO Chain
description: Example code for the eth_newPendingTransactionFilter ws method. Сomplete guide on how to use eth_newPendingTransactionFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x5cc7d95b6968d3a72c0f62a1b5b4d32c"
}
```

