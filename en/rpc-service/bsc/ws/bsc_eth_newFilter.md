---
title: bsc:eth_newFilter - Binance Smart Chain
description: Example code for the bsc:eth_newFilter ws method. Сomplete guide on how to use bsc:eth_newFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{"topics": ["0xb7407a6d74c6472bf99c4c9abe0860dc439469421c42c060639733b2309b05c7"]}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xdd078ab5685f7a3f972349ec18f02da5"
}
```

