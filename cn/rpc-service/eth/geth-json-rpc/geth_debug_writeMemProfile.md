---
title: geth:debug_writeMemProfile \[POST\] {disallowed}
description: Writes an allocation profile to the given file. Note that the profilingrate cannot be set through the API, it must be set on the command lineusing the --pprof.memprofilerate flag.
---

### Parameters


`file` - string

address of a local file.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_writeMemProfile",
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

