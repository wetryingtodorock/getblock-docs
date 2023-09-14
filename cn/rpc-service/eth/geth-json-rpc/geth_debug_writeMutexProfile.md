---
title: geth:debug_writeMutexProfile \[POST\] {disallowed}
description: Writes a goroutine blocking profile to the given file.
---

### Parameters


`file` - string

address of a local files.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_writeMutexProfile",
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

