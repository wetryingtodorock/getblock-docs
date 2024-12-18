---
title: eth_getCode - Ethereum
description: Example code for the eth_getCode ws method. Сomplete guide on how to use eth_getCode ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

20-byte contract address.

`QUANTITY|TAG` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getCode",
"params": ["0xa50a51c09a5c451c52bb714527e1974b686d8e77", "latest"],
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

