---
title: ibft_discardValidatorVote  {disallowed} - Ethereum Classic
description: Example code for the ibft_discardValidatorVote  {disallowed} json-rpc method. Сomplete guide on how to use ibft_discardValidatorVote  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

20-byte address of proposed validator.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ibft_discardValidatorVote",
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
