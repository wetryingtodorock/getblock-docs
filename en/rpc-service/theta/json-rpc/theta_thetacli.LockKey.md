---
title: theta:thetacli.LockKey \[POST\] {disallowed}
description: This API locks an account. A locked account cannot send out Theta/TFueltokens.
---

### Parameters


`address` - string

The address of the account to be locked

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "thetacli.LockKey",
"params": {},
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

