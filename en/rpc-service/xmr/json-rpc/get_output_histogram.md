---
title: xmr:get_output_histogram  {disallowed} - Monero
description: Example code for the xmr:get_output_histogram  {disallowed} json-rpc method. Сomplete guide on how to use xmr:get_output_histogram  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters

`amounts` - list of unsigned int

`min_count` - unsigned int

`max_count` - unsigned int

`unlocked` - boolean

`recent_cutoff` - unsigned int

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_output_histogram",
"params": {"amounts": 20000000000},
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
