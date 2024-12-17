---
title: eth_getTransactionCount - Gnosis
description: Example code for the eth_getTransactionCount ws method. Сomplete guide on how to use eth_getTransactionCount ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

20-byte account address.

`quantity|tag` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionCount",
"params": ["0xc94770007dda54cF92009BFF0dE90c06F603a09f", "latest"],
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

