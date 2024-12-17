---
title: eth_newBlockFilter - Avalanche
description: Example code for the eth_newBlockFilter ws method. Сomplete guide on how to use eth_newBlockFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x19d8e7f24ed667ab10f16c0b74ff41ac"
}
```

