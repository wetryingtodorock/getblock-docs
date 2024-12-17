---
title: sol:getLatestBlockhash \[POST\] {disallowed}
description: NEW This method is only available in solana-core v1.9 or newer. Pleaseuse getRecentBlockhash for solana-core v1.8Returns the latest blockhash
---

### Parameters


`commitment` - object

Optional.

Used for retrieving blockhash.

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getLatestBlockhash",
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

