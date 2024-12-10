---
title: bsv:importmulti  {disallowed} - Bitcoin SV
description: Example code for the bsv:importmulti  {disallowed} json-rpc method. Сomplete guide on how to use bsv:importmulti  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`requests` - json array, required

Data to be imported

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "importmulti",
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

