---
title: heco:eth_getBlockTransactionCountByHash \[WebSocket\]
description: Returns the number of transactions in a block from a block matching thegiven block hash.
---

### Parameters


`DATA` - string

hash of the block.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x779f94a2fad68383ed932e9f8fd04234a92b85f9d849bec2188c675dcdb0f16d"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x24"
}
```

