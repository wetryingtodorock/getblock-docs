---
title: kcc:eth_getCompilers  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:eth_getCompilers  {disallowed} ws method. Сomplete guide on how to use kcc:eth_getCompilers  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getCompilers",
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

