---
title: eth_estimateGas - Gnosis
description: Example code for the eth_estimateGas ws method. Сomplete guide on how to use eth_estimateGas ws in GetBlock.io Web3 documentation.
---

### Parameters


`object` - object

Transaction call object.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_estimateGas",
"params": [{"from": "0xFE3B557E8Fb62b89F4916B721be55cEb828dBd73", "to": "0x44Aa93095D6749A706051658B970b941c72c1D53", "value": "0x1"}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5208"
}
```

