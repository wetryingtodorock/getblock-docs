---
title: bsv:walletpassphrasechange \[POST\] {disallowed}
description: Changes the wallet passphrase from ‘oldpassphrase’ to ‘newpassphrase’.
---

### Parameters


`oldpassphrase` - string, required

The current passphrase

`newpassphrase` - string, required

The new passphrase

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' / 
--header 'x-api-key: YOUR-API-KEY' / 
--header 'Content-Type: application/json' / 
--data-raw '{"jsonrpc": "2.0",
"method": "walletpassphrasechange",
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

