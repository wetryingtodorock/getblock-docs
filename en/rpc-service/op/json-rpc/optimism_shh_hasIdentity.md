---
title: optimism:shh_hasIdentity  {disallowed} - Optimism
description: Example code for the optimism:shh_hasIdentity  {disallowed} json-rpc method. Сomplete guide on how to use optimism:shh_hasIdentity  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`address` - data

the address of the new identiy.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "shh_hasIdentity",
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

