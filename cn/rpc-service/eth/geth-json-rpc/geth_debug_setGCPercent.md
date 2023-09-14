---
title: geth:debug_setGCPercent \[POST\] {disallowed}
description: Sets the garbage collection target percentage. A negative value disablesgarbage collection.
---

### Parameters


`v` - int

garbage collector percentage

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_setGCPercent",
"params": [10],
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

