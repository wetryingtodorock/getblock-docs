---
title: eth_uninstallFilter - Moonbeam
description: Example code for the eth_uninstallFilter json-rpc method. Сomplete guide on how to use eth_uninstallFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0xb"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "Filter id 11 does not exist."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```
