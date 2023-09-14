---
title: btg:getchaintxstats \[POST\]
description: Compute statistics about the total number and rate of transactions inthe chain.
---

### Parameters


`nblocks` - numeric, optional, default=one month

Size of the window in number of blocks

`blockhash` - string, optional, default=chain tip

The hash of the block that ends the window.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getchaintxstats",
"params": [null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "time": 1631009439,
        "txcount": 267125509,
        "txrate": 0.008025484826468452,
        "window_block_count": 4320,
        "window_final_block_hash": "000000007cc1fc836d0992202730ca71f77a8cf2a35974ca300dadbf8bc1e090",
        "window_interval": 2594485,
        "window_tx_count": 20822
    }
}
```

