---
title: eth_getBlockTransactionCountByNumber - Optimism
description: Example code for the eth_getBlockTransactionCountByNumber json-rpc method. Сomplete guide on how to use eth_getBlockTransactionCountByNumber json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://optimism.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["0xc6f437"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1"
}
```

