---
title: eth:eth_submitWork \[POST\]
description: Submits a Proof of Work (Ethash) solution.Used by mining software such as Ethminer.
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

