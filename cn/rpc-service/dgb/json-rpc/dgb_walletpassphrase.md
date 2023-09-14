---
title: dgb:walletpassphrase \[POST\] {disallowed}
description: Stores the wallet decryption key in memory for ‘timeout’ seconds.This is needed prior to performing transactions related to private keyssuch as sending bitcoins Note\\Issuing the walletpassphrase command while the wallet is alreadyunlocked will set a new unlock time that overrides the old one.
---

### Parameters


`passphrase` - string, required

The wallet passphrase

`timeout` - numeric, required

The time to keep the decryption key in seconds; capped at 100000000 (~3
years).

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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

