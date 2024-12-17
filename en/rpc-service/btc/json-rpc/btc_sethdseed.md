---
title: btc:sethdseed \[POST\] {disallowed}
description: Set or generate a new HD wallet seed. Non-HD wallets will not beupgraded to being a HD wallet. Wallets that are already HD will have anew HD seed set so that new keys added to the keypool will be derivedfrom this new seed.Note that you will need to MAKE A NEW BACKUP of your wallet aftersetting the HD wallet seed.Requires wallet passphrase to be set with walletpassphrase call ifwallet is encrypted.
---

### Parameters


`newkeypool` - boolean, optional, default=true

Whether to flush old unused addresses, including change addresses, from
the keypool and regenerate it.

`seed` - string, optional, default=random seed

The WIF private key to use as the new HD seed.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "sethdseed",
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

