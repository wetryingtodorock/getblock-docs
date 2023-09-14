---
title: geth:debug_verbosity \[POST\] {disallowed}
description: Sets the logging verbosity ceiling. Log messages with level up to andincluding the given level will be printed.The verbosity of individual packages and source files can be raisedusing debug_vmodule.
---

### Parameters


`level` - number

debug level

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_verbosity",
"params": [info],
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

