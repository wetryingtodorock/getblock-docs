---
title: eth_unsubscribe - Avalanche
description: Example code for the eth_unsubscribe json-rpc method. Сomplete guide on how to use eth_unsubscribe json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

A subscription ID previously generated with eth_subscribe method.

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_unsubscribe",
"params": ["0xe5af64ddfd365b4632988c5935cfedb7"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "subscription not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```
