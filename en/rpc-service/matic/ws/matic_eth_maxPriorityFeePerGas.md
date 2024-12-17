---
title: eth_maxPriorityFeePerGas - Polygon
description: Example code for the eth_maxPriorityFeePerGas ws method. Сomplete guide on how to use eth_maxPriorityFeePerGas ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_maxPriorityFeePerGas",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x6fc23ac00"
}
```

