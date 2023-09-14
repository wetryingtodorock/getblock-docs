---
title: geth:personal_importRawKey \[POST\] {disallowed}
description: Imports the given unencrypted private key (hex string) into the keystore, encrypting it with the passphrase.Returns the address of the new account.
---

### Parameters


`keydata` - string

None

`passphrase` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_importRawKey",
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

