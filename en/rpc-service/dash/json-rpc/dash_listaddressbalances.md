---
title: dash:listaddressbalances  {disallowed} - Dash
description: Example code for the dash:listaddressbalances  {disallowed} json-rpc method. Сomplete guide on how to use dash:listaddressbalances  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Minimum Amount` - numeric (int)

Optional.

Minimum balance in DASH an address should have to be shown in the list
(default=0).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listaddressbalances",
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

