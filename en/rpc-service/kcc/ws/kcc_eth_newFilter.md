---
title: kcc:eth_newFilter - KuCoin Community Chain
description: Example code for the kcc:eth_newFilter ws method. Сomplete guide on how to use kcc:eth_newFilter ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x6448bbaaf039f88759b09f224763247c"
}
```

