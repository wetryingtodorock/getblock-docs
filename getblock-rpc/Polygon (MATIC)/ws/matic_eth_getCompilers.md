---
title: eth_getCompilers  {disallowed} - Polygon
description: Example code for the eth_getCompilers  {disallowed} ws method. Сomplete guide on how to use eth_getCompilers  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
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

