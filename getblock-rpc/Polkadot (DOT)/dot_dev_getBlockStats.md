---
title: dev_getBlockStats  {disallowed} - Polkadot
description: Example code for the dev_getBlockStats  {disallowed} json-rpc method. Сomplete guide on how to use dev_getBlockStats  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`at` - Hash

block hash

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dev_getBlockStats",
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
