---
title: etc:ibft_getValidatorsByBlockNumber  {disallowed} - Ethereum Classic
description: Example code for the etc:ibft_getValidatorsByBlockNumber  {disallowed} json-rpc method. Сomplete guide on how to use etc:ibft_getValidatorsByBlockNumber  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ibft_getValidatorsByBlockNumber",
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

