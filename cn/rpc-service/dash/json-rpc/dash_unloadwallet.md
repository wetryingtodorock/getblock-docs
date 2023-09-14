---
title: dash:unloadwallet \[POST\] {disallowed}
description: Unloads the wallet referenced by the request endpoint otherwise unloadsthe wallet specified in the argument. Specifying the wallet name on awallet endpoint is invalid.
---

### Parameters


`Filename` - string

The name of the wallet to unload.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "unloadwallet",
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

