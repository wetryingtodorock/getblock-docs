---
title: eth_getCode - Gnosis
description: Example code for the eth_getCode ws method. Сomplete guide on how to use eth_getCode ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

20-byte contract address.

`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0x3df33217f0f82c99ff3ff448512f22cef39cc208", "latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x"
}
```

