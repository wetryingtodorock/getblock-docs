---
title: sol:getFeeCalculatorForBlockhash \[POST\] {disallowed}
description: DEPRECATED Please use isBlockhashValid or getFeeForMessage instead Thismethod is expected to be removed in solana-core v2.0Returns the fee calculator associated with the query blockhash, or nullif the blockhash has expired
---

### Parameters


`blockhash` - string

query blockhash as a Base58 encoded string

`commitment` - object

Optional

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getFeeCalculatorForBlockhash",
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

