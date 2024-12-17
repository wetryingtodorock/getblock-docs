---
title: eth_maxPriorityFeePerGas  {disallowed} - Avalanche
description: Example code for the eth_maxPriorityFeePerGas  {disallowed} ws method. Сomplete guide on how to use eth_maxPriorityFeePerGas  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_maxPriorityFeePerGas",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

