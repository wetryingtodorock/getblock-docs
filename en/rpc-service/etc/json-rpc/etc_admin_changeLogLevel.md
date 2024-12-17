---
title: etc:admin_changeLogLevel \[POST\] {disallowed}
description: Changes the log level without restarting Besu. You can change the loglevel for all logs, or you can change the log level for specificpackages or classes.You can specify only one log level per RPC call.
---

### Parameters


`level` - None

Log level

`log_filter` - Array

Packages or classes to change the log level for. Optional.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_changeLogLevel",
"params": ["DEBUG", null],
"id": "getblock.io"}'
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

