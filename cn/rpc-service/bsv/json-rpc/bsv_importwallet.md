---
title: bsv:importwallet \[POST\] {disallowed}
description: Imports keys from a wallet dump file (see dumpwallet). Requires a newwallet backup to include imported keys.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`filename` - string, required

The wallet file

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "importwallet",
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

