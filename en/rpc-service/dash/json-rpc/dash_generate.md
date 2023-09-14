---
title: dash:generate \[POST\] {disallowed}
description: Since Dash Core 0.14, this RPC is not available in the officialWindows/Mac binaries. The Linux binary and binaries self-compiled (withthe appropriate options) continue to support this feature. See PR #2778for additional details.Mines blocks immediately (before the RPC call returns).
---

### Parameters


`numblocks` - number (int)

The number of blocks to generate. The RPC call will not return until all
blocks have been generated.

`maxtries` - number (int)

The number of iterations to try (default = 1000000).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "generate",
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

