---
title: admin.stopCPUProfiler  {disallowed} - Avalanche
description: Example code for the admin.stopCPUProfiler  {disallowed} ws method. Сomplete guide on how to use admin.stopCPUProfiler  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin.stopCPUProfiler",
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

