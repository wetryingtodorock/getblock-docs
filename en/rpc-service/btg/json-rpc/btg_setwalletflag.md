---
title: btg:setwalletflag  {disallowed} - Bitcoin Gold
description: Example code for the btg:setwalletflag  {disallowed} json-rpc method. Сomplete guide on how to use btg:setwalletflag  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

