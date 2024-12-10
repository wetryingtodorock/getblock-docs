---
title: heco:eth_compileSolidity  {disallowed} - Huobi ECO Chain
description: Example code for the heco:eth_compileSolidity  {disallowed} json-rpc method. Сomplete guide on how to use heco:eth_compileSolidity  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`code` - string

The source code.

### Request

``` java
curl --location --request POST 'https://heco.getblock.io/mainnet/' 
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

