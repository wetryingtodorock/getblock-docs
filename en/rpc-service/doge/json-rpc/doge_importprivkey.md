---
title: doge:importprivkey \[POST\] {disallowed}
description: import private key \[privkey\] to account \[account\], optionallyrescanning blockchain .
---

### Parameters


`privkey` - string

private key to import.

`account` - string

name of account to associate with private key.

`rescan` - boolean

Optional, default=true

rescan blockchain for transcations containing altcoin address associated
with privkey.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "importprivkey",
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

