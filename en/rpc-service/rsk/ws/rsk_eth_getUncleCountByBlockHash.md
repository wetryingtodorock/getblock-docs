---
title: eth_getUncleCountByBlockHash - Rootstock
description: Example code for the eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xf2a2b854721d4372474fc76cc13445a73369c0c334f4935c88bde3c310f28c9a"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

