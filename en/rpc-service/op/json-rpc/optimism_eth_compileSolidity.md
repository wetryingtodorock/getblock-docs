---
title: optimism:eth_compileSolidity  {disallowed} - Optimism
description: Example code for the optimism:eth_compileSolidity  {disallowed} json-rpc method. Сomplete guide on how to use optimism:eth_compileSolidity  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_compileSolidity",
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

