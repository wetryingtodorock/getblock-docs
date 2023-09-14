---
title: zec:z_getbalance \[POST\] {disallowed}
description: Returns the balance of a taddr or zaddr belonging to the nodes wallet.CAUTION If the wallet has only an incoming viewing key for thisaddress, then spends cannot be detected, and so the returned balance maybe larger than the actual balance.
---

### Parameters


`address` - string

The selected address. It may be a transparent or private address.

`minconf` - numeric

Optional, default=1

Only include transactions confirmed at least this many times.

`inZat` - boolean

Optional, default=false

Get the result amount in zatoshis (as an integer).

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_getbalance",
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

