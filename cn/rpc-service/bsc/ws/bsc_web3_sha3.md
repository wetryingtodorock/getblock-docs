---
title: bsc:web3_sha3 \[WebSocket\]
description: Returns a SHA3 hash of the specified data. The result value is aKeccak-256 hash, not the standardized SHA3-256.
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

