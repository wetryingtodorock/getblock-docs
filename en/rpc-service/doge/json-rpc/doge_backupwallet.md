---
title: doge:backupwallet \[POST\] {disallowed}
description: Safely copies wallet.dat to destination, which can be a directory or apath with filename.
---

### Parameters


`destination` - string

directory or path with filename to backup wallet to.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "backupwallet",
"params": [null],
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

