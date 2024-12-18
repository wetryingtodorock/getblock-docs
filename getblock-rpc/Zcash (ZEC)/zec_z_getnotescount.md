---
title: z_getnotescount  {disallowed} - Zcash
description: Example code for the z_getnotescount  {disallowed} json-rpc method. Сomplete guide on how to use z_getnotescount  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

