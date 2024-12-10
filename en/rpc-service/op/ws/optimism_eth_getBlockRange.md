---
title: optimism:eth_getBlockRange  {disallowed} - Optimism
description: Example code for the optimism:eth_getBlockRange  {disallowed} ws method. Сomplete guide on how to use optimism:eth_getBlockRange  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

integer of the starting block number for the range, or the string
"earliest", "latest" or "pending"

`QUANTITY|TAG` - string

integer of the ending block number for the range, or the string
"earliest", "latest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockRange",
"params": ["earliest", "latest", false],
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

