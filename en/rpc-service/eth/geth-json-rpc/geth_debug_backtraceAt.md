---
title: geth:debug_backtraceAt \[POST\] {disallowed}
description: Sets the logging backtrace location. When a backtrace location is setand a log message is emitted at that location, the stack of thegoroutine executing the log statement will be printed to stderr.
---

### Parameters


`location` - string

The location is specified as filename:line.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_backtraceAt",
"params": [filename:line],
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

