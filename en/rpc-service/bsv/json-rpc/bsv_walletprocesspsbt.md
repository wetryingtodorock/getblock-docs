---
title: bsv:walletprocesspsbt \[POST\] {disallowed}
description: Update a PSBT with input information from our wallet and then signinputs that we can sign for.Requires wallet passphrase to be set with walletpassphrase call ifwallet is encrypted.
---

### Parameters


`psbt` - string, required

The transaction base64 string

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
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

