---
title: sol:isBlockhashValid  {disallowed} - Solana
description: Example code for the sol:isBlockhashValid  {disallowed} json-rpc method. Сomplete guide on how to use sol:isBlockhashValid  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockhash` - stirng

the blockhash of this block, as base-58 encoded string

`commitment` - object

Optional

commitment (used for retrieving blockhash)

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "isBlockhashValid",
"params": ["J7rBdM6AecPDEZp8aPq5iPSNKVkU5Q76F3oAV4eW5wsW", null],
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

