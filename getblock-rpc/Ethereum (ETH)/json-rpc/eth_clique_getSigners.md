---
title: clique_getSigners  {disallowed} - Ethereum
description: Example code for the clique_getSigners  {disallowed} json-rpc method. Сomplete guide on how to use clique_getSigners  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSigners",
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

