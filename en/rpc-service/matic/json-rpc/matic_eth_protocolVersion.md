---
title: matic:eth_protocolVersion - Polygon
description: Example code for the matic:eth_protocolVersion json-rpc method. Сomplete guide on how to use matic:eth_protocolVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://matic.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_protocolVersion",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_protocolVersion does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

