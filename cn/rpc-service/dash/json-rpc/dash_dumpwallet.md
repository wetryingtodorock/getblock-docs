---
title: dash:dumpwallet \[POST\] {disallowed}
description: Creates or overwrites a file with all wallet keys in a human-readableformat.
---

### Parameters


`Filename` - string

The filename with path (either absolute or relative to Dash Core) into
which the wallet dump will be placed. An existing file with that name
will be overwritten.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dumpwallet",
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

