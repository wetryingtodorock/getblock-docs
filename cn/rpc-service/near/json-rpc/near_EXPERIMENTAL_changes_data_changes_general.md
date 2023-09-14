---
title: near:EXPERIMENTAL_changes(data_changes_general) \[POST\] {disallowed}
description: Returns the state change details of a contract based on the key prefix(encoded to base64). Pass an empty string for this param if you wouldlike to return all state changes.
---

### Parameters


`changes_type` - string

type of changes

`account_ids` - array of string

an array of account ids

`key_prefix_base64` - string

key prefix

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

