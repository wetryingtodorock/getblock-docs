---
title: doge:walletpassphrasechange  {disallowed} - Dogecoin
description: Example code for the doge:walletpassphrasechange  {disallowed} json-rpc method. Сomplete guide on how to use doge:walletpassphrasechange  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

