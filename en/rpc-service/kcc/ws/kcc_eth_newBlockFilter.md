---
title: eth_newBlockFilter - KuCoin Community Chain
description: Example code for the eth_newBlockFilter ws method. Сomplete guide on how to use eth_newBlockFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x8fb2a597e9e3e82835b9d7bbb1acfbb6"
}
```

