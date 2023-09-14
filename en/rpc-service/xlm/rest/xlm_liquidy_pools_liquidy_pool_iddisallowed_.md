---
title: xlm:/liquidy_pools/{liquidy_pool_id} \[GET\] {disallowed}
description: The single liquidity pool endpoint provides information on a liquiditypool.
---

### Parameters


`liquidity_pool_id` - path

any, required

A unique identifier for this liquidity pool.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/liquidy_pools/None' 
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

