---
title: eth_getBlockReceipts  {disallowed} - Polygon
description: Example code for the eth_getBlockReceipts  {disallowed} ws method. Сomplete guide on how to use eth_getBlockReceipts  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA, 32 Bytes` - None

Block number in hex format or tag.

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockReceipts",
"params": ["0xacffc1"],
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

