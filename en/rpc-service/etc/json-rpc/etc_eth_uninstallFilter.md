---
title: eth_uninstallFilter - Ethereum Classic
description: Example code for the eth_uninstallFilter json-rpc method. Сomplete guide on how to use eth_uninstallFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - string

Filter ID.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
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
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```

