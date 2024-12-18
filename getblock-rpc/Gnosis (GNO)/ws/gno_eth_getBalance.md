---
title: eth_getBalance - Gnosis
description: Example code for the eth_getBalance ws method. Сomplete guide on how to use eth_getBalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

20-byte account address from which to retrieve the balance.

`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBalance",
"params": ["0xfe3b557e8fb62b89f4916b721be55ceb828dbd73", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x3e20"
}
```

