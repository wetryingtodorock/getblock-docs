---
title: eth_uninstallFilter - Ethereum
description: Example code for the eth_uninstallFilter ws method. Сomplete guide on how to use eth_uninstallFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Filter ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_uninstallFilter",
"params": ["0xb"],
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

