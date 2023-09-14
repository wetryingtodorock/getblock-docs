---
title: geth:debug_startCPUProfile \[POST\] {disallowed}
description: Turns on CPU profiling indefinitely, writing to the given file.
---

### Parameters


`file` - string

address to a local file.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_startCPUProfile",
"params": ["/address/to-file"],
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

