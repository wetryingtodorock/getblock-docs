---
title: zec:z_getnotescount \[POST\] {disallowed}
description: Returns the number of sprout and sapling notes available in the wallet.
---

### Parameters


`minconf` - numeric

Optional, default=1

Only include notes in transactions confirmed at least this many times.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_getnotescount",
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

