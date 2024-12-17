---
title: eth_getBalance - KuCoin Community Chain
description: Example code for the eth_getBalance json-rpc method. Сomplete guide on how to use eth_getBalance json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address to check for balance.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "latest"],
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

