---
title: xmr:get_fee_estimate \[POST\]
description: Gives an estimation on fees per byte.
---

### Parameters

`grace_blocks` - unsigned int

Optional

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_fee_estimate",
"params": {},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "credits": 0,
        "fee": 6407,
        "quantization_mask": 10000,
        "status": "OK",
        "top_hash": "",
        "untrusted": false
    }
}
```
