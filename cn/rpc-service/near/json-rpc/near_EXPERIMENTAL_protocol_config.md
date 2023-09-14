---
title: near:EXPERIMENTAL_protocol_config \[POST\] {disallowed}
description: Returns most recent protocol configuration or a specific queried block.Useful for finding current storage and transaction costs.
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
"method": "EXPERIMENTAL_protocol_config",
"params": ["final", null],
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

