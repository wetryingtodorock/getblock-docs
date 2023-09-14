---
title: xlm:/liquidy_pools \[GET\] {disallowed}
description: This endpoint lists all available liquidity pools.
---

### Parameters


`reserves` - query

any, optional

Comma-separated list of assets in canonical form (Code:IssuerAccountID),
to only include liquidity pools which have reserves matching all listed
assets.

`account` - query

any, optional

A Stellar account ID, to only include liquidity pools in which this
account is participating in (i.e. holds pool shares to).

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/liquidy_pools' 
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

