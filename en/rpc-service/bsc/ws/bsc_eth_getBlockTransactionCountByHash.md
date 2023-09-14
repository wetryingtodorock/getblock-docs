---
title: bsc:eth_getBlockTransactionCountByHash \[WebSocket\]
description: Returns the number of transactions in the block matching the given blockhash.
---

### Parameters


`data` - hex string

32-byte block hash.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByHash",
"params": ["0x51da5dc897ffaa4754e2cd84b59c4701abbef43d66abac1fc5c9a2bcaf3455f3"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x121"
}
```

