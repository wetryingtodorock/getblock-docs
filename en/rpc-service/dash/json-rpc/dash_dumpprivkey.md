---
title: dash:dumpprivkey  {disallowed} - Dash
description: Example code for the dash:dumpprivkey  {disallowed} json-rpc method. Сomplete guide on how to use dash:dumpprivkey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`P2PKH Address` - string (base58)

The P2PKH address corresponding to the private key you want returned.
Must be the address corresponding to a private key in this wallet.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dumpprivkey",
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

