---
title: doge:walletpassphrasechange \[POST\] {disallowed}
description: Changes the wallet passphrase from \[oldpassphrase\] to\[newpassphrase\].
---

### Parameters


`oldphrase` - string

The old passphrase.

`newphrase` - string

The new passphrase.

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
"method": "walletpassphrasechange",
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

