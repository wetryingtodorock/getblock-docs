---
title: near:EXPERIMENTAL_changes(data_changes_deploy)  {disallowed} - NEAR Protocol
description: Example code for the near:EXPERIMENTAL_changes(data_changes_deploy)  {disallowed} json-rpc method. Сomplete guide on how to use near:EXPERIMENTAL_changes(data_changes_deploy)  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`changes_type` - string

type of changes

`account_ids` - array of string

an array of account ids

`block_id` - int

block id

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "EXPERIMENTAL_changes",
"params": {"changes_type": "data_changes"},
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

