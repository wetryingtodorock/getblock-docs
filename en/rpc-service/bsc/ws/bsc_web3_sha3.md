---
title: web3_sha3 - Binance Smart Chain
description: Example code for the web3_sha3 ws method. Сomplete guide on how to use web3_sha3 ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

Data to convert to a SHA3 hash.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "web3_sha3",
"params": ["0x68656c6c6f20776f726c00"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5e39a0a66544c0668bde22d61c47a8710000ece931f13b84d3b2feb44ec96d3f"
}
```

