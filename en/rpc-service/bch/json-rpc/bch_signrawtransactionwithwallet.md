---
title: bch:signrawtransactionwithwallet  {disallowed} - Bitcoin Cash
description: Example code for the bch:signrawtransactionwithwallet  {disallowed} json-rpc method. Сomplete guide on how to use bch:signrawtransactionwithwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hexstring` - string, required

The transaction hex string

`prevtxs` - json array, optional

The previous dependent transaction outputs

`sighashtype` - string, optional, default=ALL

“ALL” “NONE” “SINGLE” “ALL\|ANYONECANPAY” “NONE\|ANYONECANPAY”
“SINGLE\|ANYONECANPAY”

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "signrawtransactionwithwallet",
"params": [null, null, null],
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

