---
title: admin.setLogLevel  {disallowed} - Avalanche
description: Example code for the admin.setLogLevel  {disallowed} ws method. Сomplete guide on how to use admin.setLogLevel  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`level` - string

level is the log level to be set.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin.setLogLevel",
"params": ["info"],
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

