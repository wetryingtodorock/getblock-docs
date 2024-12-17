---
title: dash:encryptwallet \[POST\] {disallowed}
description: Encrypts the wallet with a passphrase. This is only to enable encryptionfor the first time. After encryption is enabled, you will need to enterthe passphrase to use private keys.if using this RPC on the command line, remember that your shell probablysaves your command lines (including the value of the passphraseparameter). In addition, there is no RPC to completely disableencryption. If you want to return to an unencrypted wallet, you mustcreate a new wallet and restore your data from a backup made with thedumpwallet RPC.
---

### Parameters


`Passphrase` - string

The passphrase to use for the encrypted wallet. Must be at least one
character.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
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

