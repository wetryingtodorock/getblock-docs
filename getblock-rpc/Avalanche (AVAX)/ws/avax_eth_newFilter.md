---
title: eth_newFilter - Avalanche
description: Example code for the eth_newFilter ws method. Сomplete guide on how to use eth_newFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{"fromBlock": "earliest", "toBlock": "latest", "topics": []}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x149c3e3f7a44b70568d865d6fd58c619"
}
```

