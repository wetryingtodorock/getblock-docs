---
title: etc:eth_getWork - Ethereum Classic
description: Example code for the etc:eth_getWork json-rpc method. Сomplete guide on how to use etc:eth_getWork json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
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
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0xce5e32ca59cb86799a1879e90150b2c3b882852173e59865e9e79abb67a9d636",
        "0x0000000000000000000000000000000000000000000000000000000000000000",
        "0x00a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3d70a3",
        "0x42"
    ]
}
```

