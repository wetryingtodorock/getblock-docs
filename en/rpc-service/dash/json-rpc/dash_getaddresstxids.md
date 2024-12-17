---
title: getaddresstxids  {disallowed} - Dash
description: Example code for the getaddresstxids  {disallowed} json-rpc method. Сomplete guide on how to use getaddresstxids  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`addresses` - object

An array of P2PKH or P2SH Dash address(es).

`start` - number (int)

Optional.

The start block height

`end` - number (int)

Optional.

The end block height

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddresstxids",
"params": [[{"name": "address", "type": "string (base58)", "description": ["The base58check encoded address."], "value": null}], null, null],
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

