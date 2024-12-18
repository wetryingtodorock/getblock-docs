---
title: eth_uninstallFilter - Binance Smart Chain
description: Example code for the eth_uninstallFilter ws method. Сomplete guide on how to use eth_uninstallFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0x6b08f09a8c82c83da98981500efd5540"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": false
}
```

