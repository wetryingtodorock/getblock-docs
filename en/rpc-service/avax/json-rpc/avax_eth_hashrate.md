---
title: avax:eth_hashrate \[POST\]
description: Returns the number of hashes per second that the node is mining with.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_hashrate",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_hashrate does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

