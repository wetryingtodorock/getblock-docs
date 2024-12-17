---
title: kcc:eth_getWork  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:eth_getWork  {disallowed} ws method. Сomplete guide on how to use kcc:eth_getWork  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getWork",
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

