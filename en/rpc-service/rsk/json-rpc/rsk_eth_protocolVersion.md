---
title: rsk:eth_protocolVersion - Rootstock
description: Example code for the rsk:eth_protocolVersion json-rpc method. Сomplete guide on how to use rsk:eth_protocolVersion json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_protocolVersion",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "62"
}
```

