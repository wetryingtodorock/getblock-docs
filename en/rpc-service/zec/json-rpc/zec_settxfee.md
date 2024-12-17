---
title: settxfee  {disallowed} - Zcash
description: Example code for the settxfee  {disallowed} json-rpc method. Сomplete guide on how to use settxfee  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`amount` - numeric

The transaction fee in ZEC/kB rounded to the nearest 0.00000001

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "settxfee",
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

