---
title: bch:walletprocesspsbt  {disallowed} - Bitcoin Cash
description: Example code for the bch:walletprocesspsbt  {disallowed} json-rpc method. Сomplete guide on how to use bch:walletprocesspsbt  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`psbt` - string, required

The transaction base64 string

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "walletprocesspsbt",
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

