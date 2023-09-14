---
title: sol:getRecentBlockhash \[POST\] {disallowed}
description: DEPRECATED Please use getLatestBlockhash instead This method isexpected to be removed in solana-core v2.0Returns a recent block hash from the ledger, and a fee schedule that canbe used to compute the cost of submitting a transaction using it.
---

### Parameters


`commitment` - object

optional

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getRecentBlockhash",
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

