---
title: dumpprivkey  {disallowed} - Zcash
description: Example code for the dumpprivkey  {disallowed} json-rpc method. Сomplete guide on how to use dumpprivkey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`t-addr` - string

The transparent address for the private key.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
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

