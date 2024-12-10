---
title: cro:eth_getBlockTransactionCountByHash - Cronos
description: Example code for the cro:eth_getBlockTransactionCountByHash json-rpc method. Сomplete guide on how to use cro:eth_getBlockTransactionCountByHash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x08840bf78ffc1aebc8237d3c3d209f8337f0e0c2f975e5b1c3eac816d28d760e"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x3"
}
```

