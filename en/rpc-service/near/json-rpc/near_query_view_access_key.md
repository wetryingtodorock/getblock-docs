---
title: near:query(view_access_key)  {disallowed} - NEAR Protocol
description: Example code for the near:query(view_access_key)  {disallowed} json-rpc method. Сomplete guide on how to use near:query(view_access_key)  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

`public_key` - string

public key of an account.

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "query",
"params": ["view_access_key", "final", null, null, null],
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

