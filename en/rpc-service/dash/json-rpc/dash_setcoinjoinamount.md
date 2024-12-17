---
title: dash:setcoinjoinamount \[POST\] {disallowed}
description: Sets the amount of DASH to be processed with CoinJoin (previously namedsetprivatesendamount prior to Dash Core 0.17.0).
---

### Parameters


`Amount` - int

The number of DASH to process (minimum: 2, maximum: 21,000,000)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setcoinjoinamount",
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

