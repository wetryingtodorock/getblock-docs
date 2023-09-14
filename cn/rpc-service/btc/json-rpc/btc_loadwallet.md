---
title: btc:loadwallet \[POST\] {disallowed}
description: Loads a wallet from a wallet file or directory.Note that all wallet command-line options used when starting bitcoindwill be applied to the new wallet (eg -rescan, etc).
---

### Parameters


`filename` - string, required

The wallet directory or .dat file.

`load_on_startup` - boolean, optional, default=null

Save wallet name to persistent settings and load on startup. True to add
wallet to startup list, false to remove, null to leave unchanged.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "loadwallet",
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

