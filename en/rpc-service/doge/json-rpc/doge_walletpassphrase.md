---
title: doge:walletpassphrase \[POST\] {disallowed}
description: Stores the wallet decryption key in memory for \[timeout\] seconds.
---

### Parameters


`passphrase` - string

The wallet passphrase.

`timeout` - integer

Time in seconds to keep the wallet unlocked (by keeping the passphrase
in memory).

`dont_raise` - boolean

Optional, default=false

Instead of raising ~dogecoinrpc.exceptions.WalletPassphraseIncorrect
return False.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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

