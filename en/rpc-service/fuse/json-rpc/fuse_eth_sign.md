---
title: fuse:eth_sign - Fuse Network
description: Example code for the fuse:eth_sign json-rpc method. Сomplete guide on how to use fuse:eth_sign json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

address.

`DATA` - string

message to sign.

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sign",
"params": ["0x9b956e3d318625be2686ae7268d81777c462d41f", "0xdeadbeaf"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32041,
        "message": "Request has been rejected because of queue limit."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

