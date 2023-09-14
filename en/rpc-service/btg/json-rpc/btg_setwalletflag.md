---
title: btg:setwalletflag \[POST\] {disallowed}
description: Change the state of the given wallet flag for a wallet.
---

### Parameters


`flag` - string, required

The name of the flag to change. Current available flags - avoid_reuse

`value` - boolean, optional, default=true

The new state.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setwalletflag",
"params": [null, null],
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

