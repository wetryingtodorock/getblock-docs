---
title: eth:eth_submitWork \[WebSocket\]
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
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_submitWork",
"params": ["0x0000000000000001", "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef", "0x1234567890abcdef1234567890abcdef1234567890abcdef1234567890abcdef"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": false
}
```

