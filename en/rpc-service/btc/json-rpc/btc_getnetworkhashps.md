---
title: btc:getnetworkhashps - Bitcoin
description: Example code for the btc:getnetworkhashps json-rpc method. Сomplete guide on how to use btc:getnetworkhashps json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`nblocks` - numeric, optional, default=120

The number of blocks, or -1 for blocks since last difficulty change.

`height` - numeric, optional, default=-1

To estimate at the time of the given height.

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
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
    "result": 2.333876557488516e+18
}
```

