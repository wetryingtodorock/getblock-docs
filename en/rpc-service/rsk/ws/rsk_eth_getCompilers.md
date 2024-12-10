---
title: rsk:eth_getCompilers  {disallowed} - Rootstock
description: Example code for the rsk:eth_getCompilers  {disallowed} ws method. Сomplete guide on how to use rsk:eth_getCompilers  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
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

