---
title: eth_coinbase - Cronos
description: Example code for the eth_coinbase json-rpc method. Сomplete guide on how to use eth_coinbase json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "rpc error: code = Unknown desc = validator not found for crcvalcons1vvk5s0mvdtd6r84pd6jxuchk8ry34qhd2lyzk2"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

