---
title: ftm:eth_getFilterChanges - Fantom
description: Example code for the ftm:eth_getFilterChanges json-rpc method. Сomplete guide on how to use ftm:eth_getFilterChanges json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x7c3173bd21b6fd2ad8be24c9aa40e8d9"],
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

