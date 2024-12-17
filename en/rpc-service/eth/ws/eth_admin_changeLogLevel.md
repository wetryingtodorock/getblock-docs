---
title: eth:admin_changeLogLevel \[WebSocket\] {disallowed}
description: Changes the log level without restarting Besu. You can change the loglevel for all logs, or you can change the log level for specificpackages or classes.You can specify only one log level per RPC call.
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

