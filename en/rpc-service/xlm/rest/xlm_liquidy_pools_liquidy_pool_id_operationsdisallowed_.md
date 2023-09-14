---
title: xlm:/liquidy_pools/{liquidy_pool_id}/operations \[GET\] {disallowed}
description: This endpoint represents successful operations referencing a givenliquidity pool and can be used in streaming mode. Streaming mode allowsyou to listen for new operations referencing this liquidity pool as theyare added to the Stellar ledger. If called in streaming mode, Horizonwill start at the earliest known operation unless a cursor is set, inwhich case it will start from that cursor. By setting the cursor valueto now, you can stream operations created since your request time.
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

`include_failed` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

`join` - query

any, optional

Set to transactions to include the transactions which created each of
the operations in the response.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/liquidy_pools/None/operations?' 
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

