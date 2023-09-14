---
title: dash:walletpassphrasechange \[POST\] {disallowed}
description: Changes the wallet passphrase from old passphrase to new passphrase.If using this RPC on the command line, remember that your shell probablysaves your command lines (including the value of the passphraseparameter).
---

### Parameters


`Current Passphrase` - string

The current wallet passphrase.

`New Passphrase` - string

The new passphrase for the wallet.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "None",
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

