---
title: geth:personal_newAccount \[POST\] {disallowed}
description: Generates a new private key and stores it in the key store directory.The key file is encrypted with the given passphrase. Returns the addressof the new account.At the geth console, newAccount will prompt for a passphrase when it isnot supplied as the argument.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_newAccount",
"params": [],
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

