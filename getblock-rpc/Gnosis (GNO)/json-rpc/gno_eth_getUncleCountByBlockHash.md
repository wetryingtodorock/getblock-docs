---
title: eth_getUncleCountByBlockHash - Gnosis
description: Example code for the eth_getUncleCountByBlockHash json-rpc method. Сomplete guide on how to use eth_getUncleCountByBlockHash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

32-byte block hash.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xc11de1b67dd435ada2b83bbf0bb45cba5efab4e8dd00b100142e799ba902dddc"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

