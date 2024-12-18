---
title: gettxoutsetinfo  {disallowed} - Bitcoin SV
description: Example code for the gettxoutsetinfo  {disallowed} json-rpc method. Сomplete guide on how to use gettxoutsetinfo  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hash_type` - string, optional, default=hash_serialized_2

Which UTXO set hash should be calculated. Options 'hash_serialized_2'
(thelegacy algorithm), 'none'."

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "gettxoutsetinfo",
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

