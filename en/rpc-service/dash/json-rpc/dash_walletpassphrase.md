---
title: dash:walletpassphrase \[POST\] {disallowed}
description: Stores the wallet decryption key in memory for the indicated number ofseconds. Issuing the walletpassphrase command while the wallet isalready unlocked will set a new unlock time that overrides the old one.If using this RPC on the command line, remember that your shell probablysaves your command lines (including the value of the passphraseparameter).
---

### Parameters


`Passphrase` - string

The passphrase that unlocks the wallet.

`Seconds` - number (int)

The number of seconds after which the decryption key will be
automatically deleted from memory.

`Mixing Only` - bool

Optional.

If true, the wallet will be locked for sending functions but unlocked
for mixing transactions (default = false).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "walletpassphrase",
"params": [null, null, null],
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

