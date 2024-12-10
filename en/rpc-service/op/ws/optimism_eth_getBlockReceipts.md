---
title: optimism:eth_getBlockReceipts - Optimism
description: Example code for the optimism:eth_getBlockReceipts ws method. Сomplete guide on how to use optimism:eth_getBlockReceipts ws in GetBlock.io Web3 documentation.
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

