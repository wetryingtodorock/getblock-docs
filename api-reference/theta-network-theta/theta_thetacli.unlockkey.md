---
title: thetacli.UnlockKey  {disallowed} - Theta Network
description: Example code for the thetacli.UnlockKey  {disallowed} json-rpc method. Сomplete guide on how to use thetacli.UnlockKey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
