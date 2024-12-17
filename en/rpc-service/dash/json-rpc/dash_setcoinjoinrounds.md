---
title: dash:setcoinjoinrounds \[POST\] {disallowed}
description: Sets the number of rounds to use (previously named setprivatesendroundsprior to Dash Core 0.17.0).
---

### Parameters


`Rounds` - int

The number of rounds to use (minimum: 1, maximum: 16)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setcoinjoinrounds",
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

