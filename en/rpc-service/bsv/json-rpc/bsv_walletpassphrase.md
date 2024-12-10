---
title: bsv:walletpassphrase  {disallowed} - Bitcoin SV
description: Example code for the bsv:walletpassphrase  {disallowed} json-rpc method. Сomplete guide on how to use bsv:walletpassphrase  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`passphrase` - string, required

The wallet passphrase

`timeout` - numeric, required

The time to keep the decryption key in seconds; capped at 100000000 (~3
years).

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "walletpassphrase",
"params": [null, null],
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

