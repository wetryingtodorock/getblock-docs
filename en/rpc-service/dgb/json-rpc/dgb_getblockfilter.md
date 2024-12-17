---
title: dgb:getblockfilter - DigiByte
description: Example code for the dgb:getblockfilter json-rpc method. Сomplete guide on how to use dgb:getblockfilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockhash` - string, required

The block hash

`filtertype` - string, optional, default=basic

0 for hex-encoded data, 1 for a json object, and 2 for json object with
transaction data

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockfilter",
"params": ["8aef53e812659444b72dfa021ccbfddfb795e04889788c8dee802113e186acf3", null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

