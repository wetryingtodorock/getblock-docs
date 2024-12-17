---
title: matic:eth_unsubscribe - Polygon
description: Example code for the matic:eth_unsubscribe json-rpc method. Сomplete guide on how to use matic:eth_unsubscribe json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

A subscription ID previously generated with eth_subscribe method.

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
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

