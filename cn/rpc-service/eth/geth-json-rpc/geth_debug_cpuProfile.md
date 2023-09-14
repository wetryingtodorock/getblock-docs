---
title: geth:debug_cpuProfile \[POST\] {disallowed}
description: Turns on CPU profiling for the given duration and writes profile data todisk.
---

### Parameters


`file` - string

local file address

`seconds` - number

duration

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_cpuProfile",
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

