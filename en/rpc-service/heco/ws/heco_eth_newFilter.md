---
title: heco:eth_newFilter - Huobi ECO Chain
description: Example code for the heco:eth_newFilter ws method. Сomplete guide on how to use heco:eth_newFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x986408b4648973ee2c2490d2b054055"
}
```

