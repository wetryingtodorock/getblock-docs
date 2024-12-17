---
title: admin_changeLogLevel  {disallowed} - Ethereum
description: Example code for the admin_changeLogLevel  {disallowed} ws method. Сomplete guide on how to use admin_changeLogLevel  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`level` - None

Log level

`log_filter` - Array

Packages or classes to change the log level for. Optional.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_changeLogLevel",
"params": ["DEBUG", null],
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

