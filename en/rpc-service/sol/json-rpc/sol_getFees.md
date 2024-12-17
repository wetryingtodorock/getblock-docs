---
title: sol:getFees \[POST\] {disallowed}
description: DEPRECATED Please use getFeeForMessage instead This method is expectedto be removed in solana-core v2.0Returns a recent block hash from the ledger, a fee schedule that can beused to compute the cost of submitting a transaction using it, and thelast slot in which the blockhash will be valid.
---

### Parameters


`commitment` - object

Optional

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getFees",
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

