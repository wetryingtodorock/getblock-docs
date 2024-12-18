---
title: eth_submitWork - Ethereum
description: Example code for the eth_submitWork json-rpc method. Сomplete guide on how to use eth_submitWork json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA, 8 Bytes` - None

Retrieved nonce.

`DATA, 32 Bytes` - None

Hash of the block header (PoW-hash).

`DATA, 32 Bytes` - None

Mix digest.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_submitWork",
"params": ["0x0000000000000001", "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef", "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": false
}
```

