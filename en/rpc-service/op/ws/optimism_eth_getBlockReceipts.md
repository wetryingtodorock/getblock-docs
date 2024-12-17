---
title: optimism:eth_getBlockReceipts \[WebSocket\]
description: Returns all transaction receipts for a given block.
---

### Parameters


`DATA, 32 Bytes` - None

Block number in hex format or tag.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockReceipts",
"params": ["0xacffc1"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method eth_getBlockReceipts does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

