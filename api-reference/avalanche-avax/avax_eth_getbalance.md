---
title: eth_getBalance - Avalanche
description: Example code for the eth_getBalance json-rpc method. Сomplete guide on how to use eth_getBalance json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0x0f8d94cea1eba9c582bbe800545ca91dfc39da18", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x2fe10fc87c0ae5"
}
```

