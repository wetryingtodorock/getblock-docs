---
title: getFees  {disallowed} - Solana
description: Example code for the getFees  {disallowed} json-rpc method. Сomplete guide on how to use getFees  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
