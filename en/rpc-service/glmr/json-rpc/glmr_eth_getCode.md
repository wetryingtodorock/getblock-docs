---
title: glmr:eth_getCode - Moonbeam
description: Example code for the glmr:eth_getCode json-rpc method. Сomplete guide on how to use glmr:eth_getCode json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0xbec4e80531dad6a9989828d174cc2878b1e3123d", "latest"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```

