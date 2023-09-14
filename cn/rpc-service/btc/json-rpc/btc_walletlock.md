---
title: btc:walletlock \[POST\] {disallowed}
description: Removes the wallet encryption key from memory, locking the wallet.After calling this method, you will need to call walletpassphrase againbefore being able to call any methods which require the wallet to beunlocked.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "walletlock",
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

