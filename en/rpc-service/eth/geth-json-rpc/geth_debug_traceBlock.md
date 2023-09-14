---
title: geth:debug_traceBlock \[POST\] {disallowed}
description: The traceBlock method will return a full stack trace of all invokedopcodes of all transaction that were included in this block. Note, theparent of this block must be present or it will fail.
---

### Parameters


`blockRLP` - array of bytes

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceBlock",
"params": [null],
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

