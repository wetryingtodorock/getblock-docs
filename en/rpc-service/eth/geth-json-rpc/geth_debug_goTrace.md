---
title: geth:debug_goTrace \[POST\] {disallowed}
description: Turns on Go runtime tracing for the given duration and writes trace datato disk.
---

### Parameters


`file` - string

address of a local file.

`seconds` - number

trace duration

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_goTrace",
"params": ["/local/file", 100],
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

