---
title: eth:eth_getWork - Ethereum
description: Example code for the eth:eth_getWork json-rpc method. Сomplete guide on how to use eth:eth_getWork json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getWork",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "no mining work available yet"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

