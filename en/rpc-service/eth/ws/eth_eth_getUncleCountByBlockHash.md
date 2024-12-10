---
title: eth:eth_getUncleCountByBlockHash - Ethereum
description: Example code for the eth:eth_getUncleCountByBlockHash ws method. Сomplete guide on how to use eth:eth_getUncleCountByBlockHash ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

32-byte block hash.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleCountByBlockHash",
"params": ["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1"
}
```

