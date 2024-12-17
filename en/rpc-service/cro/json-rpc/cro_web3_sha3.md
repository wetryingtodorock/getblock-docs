---
title: cro:web3_sha3 - Cronos
description: Example code for the cro:web3_sha3 json-rpc method. Сomplete guide on how to use cro:web3_sha3 json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

Data to convert to a SHA3 hash.

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "web3_sha3",
"params": ["0x68656c6c6f20776f726c00"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xabef0720dbe9129048cb811d0f5d2d300cf6c4e4612d5acbf1ebaff090b56a7e"
}
```

