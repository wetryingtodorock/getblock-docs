---
title: ibft_getValidatorsByBlockHas  {disallowed} - Ethereum Classic
description: Example code for the ibft_getValidatorsByBlockHas  {disallowed} json-rpc method. Сomplete guide on how to use ibft_getValidatorsByBlockHas  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ibft_getValidatorsByBlockHas",
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
