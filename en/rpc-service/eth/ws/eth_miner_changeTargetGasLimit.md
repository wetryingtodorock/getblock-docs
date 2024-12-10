---
title: eth:miner_changeTargetGasLimit  {disallowed} - Ethereum
description: Example code for the eth:miner_changeTargetGasLimit  {disallowed} ws method. Сomplete guide on how to use eth:miner_changeTargetGasLimit  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity` - integer

The target gas price in Wei.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "miner_changeTargetGasLimit",
"params": [null],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

