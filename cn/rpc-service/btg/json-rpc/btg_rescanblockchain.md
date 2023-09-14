---
title: btg:rescanblockchain \[POST\] {disallowed}
description: Rescan the local blockchain for wallet related transactions.Note Use “getwalletinfo” to query the scanning progress.
---

### Parameters


`start_height` - numeric, optional, default=0

block height where the rescan should start

`stop_height` - numeric, optional

the last block height that should be scanned. If none is provided it
will rescan up to the tip at return time of this call.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "rescanblockchain",
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

