---
title: zec:getnetworksolps - Zcash
description: Example code for the zec:getnetworksolps json-rpc method. Сomplete guide on how to use zec:getnetworksolps json-rpc in GetBlock.io Web3 documentation.
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

