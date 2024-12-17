---
title: optimism:eth_getTransactionByBlockHashAndIndex - Optimism
description: Example code for the optimism:eth_getTransactionByBlockHashAndIndex json-rpc method. Сomplete guide on how to use optimism:eth_getTransactionByBlockHashAndIndex json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

Hash of a block.

`QUANTITY` - string

Transaction index position.

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockHashAndIndex",
"params": ["0x56436a935370b8decda78cf4a60e0668a882764af1cdec3a6d6967f944f4dace", "0x0"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

