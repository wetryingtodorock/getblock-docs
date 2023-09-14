---
title: zec:z_importviewingkey \[POST\] {disallowed}
description: Adds a viewing key (as returned by z_exportviewingkey) to your wallet.
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
"method": "z_importviewingkey",
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

