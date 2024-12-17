---
title: dash:setlabel  {disallowed} - Dash
description: Example code for the dash:setlabel  {disallowed} json-rpc method. Сomplete guide on how to use dash:setlabel  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Address` - string (base58)

The P2PKH or P2SH Dash address to be associated with a label.

`Label` - string

The label to assign to the address.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "setlabel",
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

