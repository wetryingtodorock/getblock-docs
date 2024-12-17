---
title: eth_getFilterChanges - Cronos
description: Example code for the eth_getFilterChanges json-rpc method. Сomplete guide on how to use eth_getFilterChanges json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x7c31"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "filter 0x7c31 not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

