---
title: bsc:eth_submitWork  {disallowed} - Binance Smart Chain
description: Example code for the bsc:eth_submitWork  {disallowed} ws method. Сomplete guide on how to use bsc:eth_submitWork  {disallowed} ws in GetBlock.io Web3 documentation.
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
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_submitWork",
"params": [1, 8234104122482341265491137074636836252947884782870784360943022469005013929455, "0xD1GE5700000000000000000000000000D1GE5700000000000000000000000000"],
"id": "getblock.io"}
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

