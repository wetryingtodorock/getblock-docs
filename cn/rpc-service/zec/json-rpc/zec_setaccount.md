---
title: zec:setaccount \[POST\] {disallowed}
description: DEPRECATED. Sets the account associated with the given address.
---

### Parameters


`zcashaddress` - string

The Zcash address to be associated with an account.

`account` - string

MUST be set to the empty string "" to represent the default account.
Passing any other string will result in an error.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setaccount",
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

