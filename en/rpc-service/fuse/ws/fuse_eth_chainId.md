---
title: fuse:eth_chainId - Fuse Network
description: Example code for the fuse:eth_chainId ws method. Сomplete guide on how to use fuse:eth_chainId ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_chainId",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x7a"
}
```

