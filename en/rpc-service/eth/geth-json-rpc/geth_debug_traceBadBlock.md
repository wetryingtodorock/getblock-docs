---
title: geth:debug_traceBadBlock \[POST\] {disallowed}
description: Returns the structured logs created during the execution of EVM againsta block pulled from the pool of bad ones and returns them as a JSONobject.
---

### Parameters


`blockHash` - string

hash of a block

`options` - array of string

additional options

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceBadBlock",
"params": ["0xe3962f0c7b342e3517a7a6e1a8c6ab51565840d93ca457caf462358ff2e612c"],
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

