---
title: get_output_distribution - Monero
description: Example code for the get_output_distribution json-rpc method. Сomplete guide on how to use get_output_distribution json-rpc in GetBlock.io Web3 documentation.

### Parameters

`amounts` - array of unsigned int

amounts to look for

`cumulative` - boolean

(optional, default is false) States if the result should be cumulative
(true) or not (false)

`from_height` - unsigned int;

(optional, default is 0) starting height to check from

`to_height` - unsigned int

(optional, default is 0) ending height to check up to

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_output_distribution",
"params": {"amounts": 628780000, "from_height": 1462078},
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "credits": 0,
        "status": "OK",
        "top_hash": "",
        "untrusted": false
    }
}
```
