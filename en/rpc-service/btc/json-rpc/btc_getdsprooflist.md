---
title: btc:getdsprooflist \[POST\] {disallowed}
description: List double-spend proofs for transactions in the mempool.
---

### Parameters


`verbosity` - numeric, optional, default=0

Values 0-3 return progressively more information for each increase in
verbosity. This option may also be specified as a boolean where false is
the same as verbosity=0 and true is verbosity=2.

`include_orphans` - boolean, optional, default=false

If true, then also include double-spend proofs that we know about but
which are for transactions that we don't yet have.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getdsprooflist",
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

