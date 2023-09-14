---
title: geth:personal_unlockAccount \[POST\] {disallowed}
description: Decrypts the key with the given address from the key store.Both passphrase and unlock duration are optional when using theJavaScript console. If the passphrase is not supplied as an argument,the console will prompt for the passphrase interactively.The unencrypted key will be held in memory until the unlock durationexpires. If the unlock duration defaults to 300 seconds. An explicitduration of zero seconds unlocks the key until geth exits.The account can be used with eth_sign and eth_sendTransaction while itis unlocked.
---

### Parameters


`adress` - string

None

`passphrase` - string

None

`duration` - number

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_unlockAccount",
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

