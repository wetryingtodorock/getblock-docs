---
title: avax:eth_compileLLL  {disallowed} - Avalanche
description: Example code for the avax:eth_compileLLL  {disallowed} json-rpc method. Сomplete guide on how to use avax:eth_compileLLL  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_compileLLL",
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

