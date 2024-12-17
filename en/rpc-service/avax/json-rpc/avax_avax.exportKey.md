---
title: avax:avax.exportKey  {disallowed} - Avalanche
description: Example code for the avax:avax.exportKey  {disallowed} json-rpc method. Сomplete guide on how to use avax:avax.exportKey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`username` - string

username must control address.

`password` - string

user's password

`address` - string

address is the address for which you want to export the corresponding
private key.

It should be in hex format.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.exportKey",
"params": [null, null, null],
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

