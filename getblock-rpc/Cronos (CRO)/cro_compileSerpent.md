---
title: compileSerpent  {disallowed} - Cronos
description: Example code for the compileSerpent  {disallowed} json-rpc method. Сomplete guide on how to use compileSerpent  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`String` - hex string

The source code.

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "compileSerpent",
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
