---
title: walletcreatefundedpsbt  {disallowed} - DigiByte
description: Example code for the walletcreatefundedpsbt  {disallowed} json-rpc method. Сomplete guide on how to use walletcreatefundedpsbt  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`inputs` - json array, optional

Leave empty to add inputs automatically. See add_inputs option.

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "walletcreatefundedpsbt",
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

