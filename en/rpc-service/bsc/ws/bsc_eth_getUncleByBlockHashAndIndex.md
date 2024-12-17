---
title: bsc:eth_getUncleByBlockHashAndIndex - Binance Smart Chain
description: Example code for the bsc:eth_getUncleByBlockHashAndIndex ws method. Сomplete guide on how to use bsc:eth_getUncleByBlockHashAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

32-byte block hash.

`quantity` - hex string

Index of the uncle.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0x94c626286c237e187454ddd993adc534f0ce3468aaec134a39fbd52185cc3a5f", "0x2"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

