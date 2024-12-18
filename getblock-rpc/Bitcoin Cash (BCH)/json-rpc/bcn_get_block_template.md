---
title: get_block_template  {disallowed} - Bitcoin Cash
description: Example code for the get_block_template  {disallowed} json-rpc method. Сomplete guide on how to use get_block_template  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`wallet_address` - string

None

### Request

``` java
curl --location --request POST 'https://bcn.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "get_block_template",
"params": {"wallet_address": "238HrUqVy8DMxHRufGEt6o1qmomTHbUp55FndtK7ABEuc2hUJQZFGjMZXNtsKQaAaZiVgnBuJgcG2Lt1ZEKcjv5s6fwStLv"},
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

