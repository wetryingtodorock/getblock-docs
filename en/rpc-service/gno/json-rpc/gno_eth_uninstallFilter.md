---
title: gno:eth_uninstallFilter - Gnosis
description: Example code for the gno:eth_uninstallFilter json-rpc method. Сomplete guide on how to use gno:eth_uninstallFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0x6b08"],
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

