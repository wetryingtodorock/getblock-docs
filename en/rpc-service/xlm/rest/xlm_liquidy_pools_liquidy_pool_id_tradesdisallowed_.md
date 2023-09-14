---
title: xlm:/liquidy_pools/{liquidy_pool_id}/trades \[GET\] {disallowed}
description: This endpoint represents successful trades fulfilled by the givenliquidity pool and can be used in streaming mode. Streaming mode allowsyou to listen for new trades referencing this liquidity pool as they areadded to the Stellar ledger. If called in streaming mode, Horizon willstart at the earliest known trade unless a cursor is set, in which caseit will start from that cursor. By setting the cursor value to now, youcan stream trade created since your request time.
---

### Parameters


`liquidity_pool_id` - path

any, required

A unique identifier for this liquidity pool.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn't
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn't designated, it defaults to 10.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/liquidy_pools/None/trades' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
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

