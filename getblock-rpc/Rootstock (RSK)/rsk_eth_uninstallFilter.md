---
title: eth_uninstallFilter - Rootstock
description: Example code for the eth_uninstallFilter json-rpc method. Сomplete guide on how to use eth_uninstallFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
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
