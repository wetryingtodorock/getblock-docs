---
title: zec:z_importkey \[POST\] {disallowed}
description: Adds a zkey (as returned by z_exportkey) to your wallet.Note This call can take minutes to complete if rescan is true.
---

### Parameters


`zkey` - string

The zkey (see z_exportkey).

`rescan` - boolean

Optional, default="whenkeyisnew"

Rescan the wallet for transactions - can be "yes", "no" or
"whenkeyisnew"

`startHeight` - numeric

Optional, default=0

Block height to start rescan from.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_importkey",
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

