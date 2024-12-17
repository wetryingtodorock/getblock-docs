---
title: zec:z_sendmany \[POST\] {disallowed}
description: Send multiple times. Amounts are decimal numbers with at most 8 digitsof precision.Change generated from one or more transparent addresses flows to a newtransparent address, while change generated from a shielded addressreturns to itself.When sending coinbase UTXOs to a shielded address, change is notallowed.The entire value of the UTXO(s) must be consumed.Before Sapling activates, the maximum number of zaddr outputs is 54 dueto transaction size limits.
---

### Parameters


`fromaddress` - string

The transparent or shielded address to send the funds from.

`amounts` - array

An array of json objects representing the amounts to send.

`minconf` - numeric,

Optional, default=1

Only include transactions confirmed at least this many times.

`fee` - numeric

Optional, default=0.00001

The fee amount to attach to this transaction.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_sendmany",
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

