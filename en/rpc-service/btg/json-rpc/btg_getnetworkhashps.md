---
title: btg:getnetworkhashps \[POST\]
description: Returns the estimated network hashes per second based on the last nblocks.Pass in \[blocks\] to override of blocks, -1 specifies since lastdifficulty change.Pass in \[height\] to estimate the network speed at the time when acertain block was found.
---

### Parameters


`nblocks` - numeric, optional, default=120

The number of blocks, or -1 for blocks since last difficulty change.

`height` - numeric, optional, default=-1

To estimate at the time of the given height.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getnetworkhashps",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": 2324661.797680737
}
```

