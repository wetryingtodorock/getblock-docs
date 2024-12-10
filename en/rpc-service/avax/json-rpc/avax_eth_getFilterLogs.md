---
title: avax:eth_getFilterLogs - Avalanche
description: Example code for the avax:eth_getFilterLogs json-rpc method. Сomplete guide on how to use avax:eth_getFilterLogs json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterLogs",
"params": ["0x16"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "filter not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

