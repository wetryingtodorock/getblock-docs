---
title: zec:z_exportwallet \[POST\] {disallowed}
description: Exports all wallet keys, for taddr and zaddr, in a human-readableformat. Overwriting an existing file is not permitted.
---

### Parameters


`filename` - string

The filename, saved in folder set by zcashd -exportdir option.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_exportwallet",
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

