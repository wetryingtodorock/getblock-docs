---
title: fuse:eth_getWork - Fuse Network
description: Example code for the fuse:eth_getWork json-rpc method. Сomplete guide on how to use fuse:eth_getWork json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
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
        "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef",
        "0x5EED00000000000000000000000000005EED0000000000000000000000000000",
        "0xd1ff1c01710000000000000000000000d1ff1c01710000000000000000000000"
    ]
}
```

