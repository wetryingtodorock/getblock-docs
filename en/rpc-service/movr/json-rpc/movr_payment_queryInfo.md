---
title: movr:payment_queryInfo  {disallowed} - Moonriver
description: Example code for the movr:payment_queryInfo  {disallowed} json-rpc method. Сomplete guide on how to use movr:payment_queryInfo  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`extrinsic` - Bytes

None

`at` - BlockHash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "payment_queryInfo",
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

