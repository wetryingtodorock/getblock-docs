---
title: geth:debug_startGoTrace \[POST\] {disallowed}
description: Starts writing a Go runtime trace to the given file.
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
"method": "debug_startGoTrace",
"params": ["/local/address"],
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

