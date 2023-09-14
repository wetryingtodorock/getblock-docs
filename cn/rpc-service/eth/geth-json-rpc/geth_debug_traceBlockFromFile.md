---
title: geth:debug_traceBlockFromFile \[POST\] {disallowed}
description: Similar to debug_traceBlock, traceBlockFromFile accepts a filecontaining the RLP of the block.
---

### Parameters


`fileName` - string

name of a local file

`options` - array of string

additional options

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceBlockFromFile",
"params": ["/local/file"],
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

