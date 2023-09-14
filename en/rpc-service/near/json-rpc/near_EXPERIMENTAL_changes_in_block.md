---
title: near:EXPERIMENTAL_changes_in_block \[POST\] {disallowed}
description: Returns changes in block for given block height or hash. You can alsouse finality param to return latest block details.
---

### Parameters


`finality` - string

You should pick either that or block_id.

Can be either "optimistic" or "final"

`block_id` - int or string

You should pick either that or finality.

The block_id param can take either the block number OR the block hash as
an argument.

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "EXPERIMENTAL_changes_in_block",
"params": [{"finality": "final"}],
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

