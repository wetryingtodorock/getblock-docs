---
title: zec:importaddress \[POST\] {disallowed}
description: Adds a script (in hex) or address that can be watched as if it were inyour wallet but cannot be used to spend.Note This call can take minutes to complete if rescan is true. If youhave the full public key, you should call importpubkey instead of this.Note If you import a non-standard raw script in hex form, outputssending to it will be treated as change, and not show up in many RPCs.
---

### Parameters


`script` - string

The hex-encoded script (or address)

`label` - string

Optional, default=""

An optional label.

`rescan` - boolean

Optional, default=false

Rescan the wallet for transactions.

`p2sh` - boolean

Optional, default=false

Add the P2SH version of the script as well

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importaddress",
"params": [null, null, null, null],
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

