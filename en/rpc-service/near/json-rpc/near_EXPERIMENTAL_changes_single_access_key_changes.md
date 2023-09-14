---
title: near:EXPERIMENTAL_changes(single_access_key_changes) \[POST\] {disallowed}
description: Returns individual access key changes in a specific block. You can querymultiple keys by passing an array of objects containing the account_idand public_key.
---

### Parameters


`changes_type` - string

type of change

`finality` - string

You should pick either that or block_id.

`block_id` - int or string

You should pick either that or finality.

The block_id param can take either the block number OR the block hash as
an argument.

`keys` - array of maps

an array of maps in format: \[{account_id, publick_key}\]

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "EXPERIMENTAL_changes",
"params": ["single_access_key_changes", "final", null, null],
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

