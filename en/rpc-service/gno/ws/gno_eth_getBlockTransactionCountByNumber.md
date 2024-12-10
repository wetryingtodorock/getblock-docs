---
title: gno:eth_getBlockTransactionCountByNumber - Gnosis
description: Example code for the gno:eth_getBlockTransactionCountByNumber ws method. Сomplete guide on how to use gno:eth_getBlockTransactionCountByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockTransactionCountByNumber",
"params": ["0x1AC46E3"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x3"
}
```

