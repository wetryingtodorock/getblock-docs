---
title: eth_compileLLL  {disallowed} - Optimism
description: Example code for the eth_compileLLL  {disallowed} json-rpc method. Сomplete guide on how to use eth_compileLLL  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
