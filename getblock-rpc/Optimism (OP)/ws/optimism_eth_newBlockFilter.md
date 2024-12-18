---
title: eth_newBlockFilter - Optimism
description: Example code for the eth_newBlockFilter ws method. Сomplete guide on how to use eth_newBlockFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x7faebec0dbb0b064921820ebae580d1a"
}
```

