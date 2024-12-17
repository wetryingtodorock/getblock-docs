---
title: zec:encryptwallet \[POST\] {disallowed}
description: WARNING encryptwallet is disabled.Encrypts the wallet with passphrase. This is for first timeencryption.After this, any calls that interact with private keys such as sending orsigningwill require the passphrase to be set prior the making these calls.Use the walletpassphrase call for this, and then walletlock call.If the wallet is already encrypted, use the walletpassphrasechange call.Note that this will shutdown the server.
---

### Parameters


`passphrase` - string

The pass phrase to encrypt the wallet with. It must be at least 1
character, but should be long.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "encryptwallet",
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

