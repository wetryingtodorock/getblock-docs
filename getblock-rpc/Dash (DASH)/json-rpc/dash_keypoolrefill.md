---
title: keypoolrefill  {disallowed} - Dash
description: Example code for the keypoolrefill  {disallowed} json-rpc method. Сomplete guide on how to use keypoolrefill  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Key Pool Size` - number (int)

Optional.

The new size of the keypool; if the number of keys in the keypool is
less than this number, new keys will be generated. Default is 1000. The
value 0 also equals the default. The value specified is for this call
only---the default keypool size is not changed.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "keypoolrefill",
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

