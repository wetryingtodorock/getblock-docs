---
title: zec:getnewaddress \[POST\] {disallowed}
description: Returns a new Zcash address for receiving payments.
---

### Parameters


`account` - string

MUST be set to the empty string "" to represent the default account.
Passing any other string will result in an error.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnewaddress",
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

