---
title: near:query(view_access_key_list) \[POST\] {disallowed}
description: Returns all access keys for a given account.
---

### Parameters


`request_type` - string

typ of request

`finality` - string

You should pick either that or block_id.

`block_id` - int or string

You should pick either that or finality.

The block_id param can take either the block number OR the block hash as
an argument.

`account_id` - string

id of an account.

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "query",
"params": ["view_access_key_list", "final", null, null],
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

