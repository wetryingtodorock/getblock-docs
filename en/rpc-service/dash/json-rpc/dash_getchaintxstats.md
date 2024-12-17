---
title: dash:getchaintxstats \[POST\]
description: Compute statistics about the total number and rate of transactions inthe chain.
---

### Parameters


`nblocks` - numeric

Optional.

Size of the window in number of blocks (default: one month).

`blockhash` - string

Optional.

The hash of the block that ends the window.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
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
        "time": 1631268126,
        "txcount": 38626270,
        "txrate": 0.1339127529836747,
        "window_block_count": 17280,
        "window_final_block_hash": "0000000000000019cd3a50eedc418372f7aa9060d6ded56a769a51a93dfe0e4a",
        "window_interval": 2723990,
        "window_tx_count": 364777
    }
}
```

