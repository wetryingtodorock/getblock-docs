---
title: eth_sendRawTransaction - Binance Smart Chain
description: Example code for the eth_sendRawTransaction ws method. Сomplete guide on how to use eth_sendRawTransaction ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Signed transaction serialized to hexadecimal format.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xf869018203e882520894f17f52151ebef6c7334fad080c5704d77216b732881bc16d674ec80000801ba02da1c48b670996dcb1f447ef9ef00b33033c48a4fe938f420bec3e56bfd24071a062e0aa78a81bf0290afbc3a9d8e9a068e6d74caa66c5e0fa8a46deaae96b0833"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "nonce too low"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

