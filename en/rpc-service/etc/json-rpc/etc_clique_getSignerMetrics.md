---
title: etc:clique_getSignerMetrics \[POST\] {disallowed}
description: Provides validator metrics for the specified rangeNumber of blocks from each validator.Block number of the last block proposed by each validator (if anyproposed in the specified range).All validators present in the last block.
---

### Parameters


`fromBlockNumber` - None

Integer representing a block number or the string tag earliest, as
described in Block Parameter.

`toBlockNumber` - None

Integer representing a block number or one of the string tags latest or
pending, as described in Block Parameter

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSignerMetrics",
"params": [null, null],
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

