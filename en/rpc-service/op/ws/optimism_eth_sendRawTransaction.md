---
title: eth_sendRawTransaction - Optimism
description: Example code for the eth_sendRawTransaction ws method. Сomplete guide on how to use eth_sendRawTransaction ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

The signed transaction data.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xf86b8184843b9aca00830164e694d7ac544f8a570c4d8764c3aabcf6870cbd960d0d80844e71d92d820118a011f7e0056924be24f37b634d67dee23ef432130444cb05f7540ee03c8ce16e3ca0228e09888bc26a748ace1392d37661e90d56ec7730368ca2d55dcdb73aa69351"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "invalid transaction: invalid sender"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

