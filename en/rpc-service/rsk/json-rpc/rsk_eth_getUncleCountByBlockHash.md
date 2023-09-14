---
title: rsk:eth_getUncleCountByBlockHash \[POST\]
description: Returns the number of uncles in a block from a block matching the givenblock hash.
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

