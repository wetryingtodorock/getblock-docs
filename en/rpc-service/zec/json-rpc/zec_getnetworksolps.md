---
title: zec:getnetworksolps \[POST\]
description: Returns the estimated network solutions per second based on the last nblocks.Pass in \[blocks\] to override number of blocks, -1 specifies overdifficulty averaging window.Pass in \[height\] to estimate the network speed at the time when acertain block was found.
---

### Parameters


`blocks` - numeric

Optional, default=120

The number of blocks, or -1 for blocks over difficulty averaging window.

`height` - numeric

Optional, default=-1

To estimate at the time of the given height.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnetworksolps",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 5297326416
}
```

