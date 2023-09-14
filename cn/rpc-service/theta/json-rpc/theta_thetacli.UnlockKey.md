---
title: theta:thetacli.UnlockKey \[POST\] {disallowed}
description: This API unlocks an account. Only unlocked accounts are allowed to sendout Theta/TFuel tokens.
---

### Parameters


`address` - string

The address of the account to be unlocked.

`password` - string

The password for the account.

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "thetacli.UnlockKey",
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

