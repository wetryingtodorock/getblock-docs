---
title: eth:eth_getFilterChanges - Ethereum
description: Example code for the eth:eth_getFilterChanges json-rpc method. Сomplete guide on how to use eth:eth_getFilterChanges json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Filter ID.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0xf8bf5598d9e04fbe84523d42640b9b0e"],
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

