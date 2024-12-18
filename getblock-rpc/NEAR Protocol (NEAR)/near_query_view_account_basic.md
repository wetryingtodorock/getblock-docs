---
title: query(view_account_basic) - NEAR Protocol
description: Example code for the query(view_account_basic) json-rpc method. Сomplete guide on how to use query(view_account_basic) json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`request_type` - string

request type

`finality` - string

You should pick either that or block_id.

Can be either "optimistic" or "final"

`block_id` - int or string

You should pick either that or finality.

The block_id param can take either the block number OR the block hash as
an argument.

`account_id` - string

account id

### Request

``` java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "query",
"params": {"request_type": "view_account", "finality": "final", "account_id": "staked.poolv1.near"},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "amount": "33945779367939674663889680026",
        "block_hash": "4BsKpcha4YcZCjy7wDs9DPWZ4q9GNe6mKF5KfCRhGfJj",
        "block_height": 61075007,
        "code_hash": "J1arLz48fgXcGyCPVckFwLnewNH6j1uw79thsvwqGYTY",
        "locked": "43032006277761885602868523789140",
        "storage_paid_at": 0,
        "storage_usage": 710635
    }
}
```

