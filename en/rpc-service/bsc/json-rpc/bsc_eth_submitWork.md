---
title: bsc:eth_submitWork \[POST\] {disallowed}
description: Submits a Proof of Work (Ethash) solution.Used by mining software such as Ethminer.
---

### Parameters


`DATA, 8 Bytes` - hex number

Retrieved nonce.

`DATA, 32 Bytes` - hex number

Hash of the block header (PoW-hash).

`DATA, 32 Bytes` - hex string

Mix digest.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_submitWork",
"params": [1, 8234104122482341265491137074636836252947884782870784360943022469005013929455, "0xD1GE5700000000000000000000000000D1GE5700000000000000000000000000"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

