---
title: xmr:get_coinbase_tx_sum \[POST\]
description: Get the coinbase amount and the fees amount for n last blocks starting at particular height
---

### Parameters

`height` - unsigned int

Block height from which getting the amounts

`count` - unsigned int

number of blocks to include in the sum

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_coinbase_tx_sum",
"params": {"height": 1563078, "count": 2},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "credits": 0,
        "emission_amount": 9387854817320,
        "emission_amount_top64": 0,
        "fee_amount": 83981380000,
        "fee_amount_top64": 0,
        "status": "OK",
        "top_hash": "",
        "untrusted": false,
        "wide_emission_amount": "0x889c7c06828",
        "wide_fee_amount": "0x138dae29a0"
    }
}
```
