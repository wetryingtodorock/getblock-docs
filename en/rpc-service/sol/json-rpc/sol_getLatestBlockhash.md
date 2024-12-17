---
title: getLatestBlockhash  {disallowed} - Solana
description: Example code for the getLatestBlockhash  {disallowed} json-rpc method. Сomplete guide on how to use getLatestBlockhash  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

