---
title: zec:importpubkey \[POST\] {disallowed}
description: Adds a public key (in hex) that can be watched as if it were in yourwallet but cannot be used to spend.Note This call can take minutes to complete if rescan is true.
---

### Parameters


`pubkey` - string

The hex-encoded public key.

`label` - string

Optional, default=""

An optional label.

`rescan` - boolean

Optional, default=false

Rescan the wallet for transactions.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importpubkey",
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

