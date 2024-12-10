---
title: bsc:trace_block - Binance Smart Chain
description: Example code for the bsc:trace_block json-rpc method. Сomplete guide on how to use bsc:trace_block json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "trace_block",
"params": ["0x6"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method trace_block does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

