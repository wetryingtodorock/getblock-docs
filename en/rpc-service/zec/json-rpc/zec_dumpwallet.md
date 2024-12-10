---
title: zec:dumpwallet  {disallowed} - Zcash
description: Example code for the zec:dumpwallet  {disallowed} json-rpc method. Сomplete guide on how to use zec:dumpwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`filename` - string

The filename, saved in folder set by zcashd -exportdir option.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dumpwallet",
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

