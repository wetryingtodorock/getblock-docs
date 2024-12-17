---
title: dash:getaddressesbylabel  {disallowed} - Dash
description: Example code for the dash:getaddressesbylabel  {disallowed} json-rpc method. Сomplete guide on how to use dash:getaddressesbylabel  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Label` - string

The name of the label associated with the addresses to get. To get
addresses from the default account, pass an empty string ("").

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressesbylabel",
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

