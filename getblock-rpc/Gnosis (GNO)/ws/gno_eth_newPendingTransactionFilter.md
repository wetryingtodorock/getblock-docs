---
title: eth_newPendingTransactionFilter - Gnosis
description: Example code for the eth_newPendingTransactionFilter ws method. Сomplete guide on how to use eth_newPendingTransactionFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0xe65"
}
```

