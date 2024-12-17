---
title: fuse:eth_sendRawTransaction - Fuse Network
description: Example code for the fuse:eth_sendRawTransaction json-rpc method. Сomplete guide on how to use fuse:eth_sendRawTransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

The signed transaction data.

### Request

``` java
curl --location --request POST 'https://fuse.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32602,
        "data": "RlpIncorrectListLen",
        "message": "Invalid RLP."
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

