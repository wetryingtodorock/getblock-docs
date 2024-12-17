---
title: bch:keypoolrefill \[POST\] {disallowed}
description: Fills the keypool.Requires wallet passphrase to be set with walletpassphrase call ifwallet is encrypted.
---

### Parameters


`newsize` - numeric, optional, default=100

The new keypool size

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "keypoolrefill",
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

