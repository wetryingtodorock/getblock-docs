---
title: bch:dumpwallet \[POST\] {disallowed}
description: Dumps all wallet keys in a human-readable format to a server-side file.This does not allow overwriting existing files.Imported scripts are included in the dumpfile, but corresponding BIP173addresses, etc. may not be added automatically by importwallet.Note that if your wallet contains keys which are not derived from yourHD seed (e.g. imported keys), these are not covered by only backing upthe seed itself, and must be backed up too (e.g. ensure you back up thewhole dumpfile).
---

### Parameters


`filename` - None

string, required

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "dumpwallet",
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

