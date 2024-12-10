---
title: kcc:eth_newPendingTransactionFilter - KuCoin Community Chain
description: Example code for the kcc:eth_newPendingTransactionFilter ws method. Сomplete guide on how to use kcc:eth_newPendingTransactionFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0xd10628575a546559edf35c7801b605e9"
}
```

