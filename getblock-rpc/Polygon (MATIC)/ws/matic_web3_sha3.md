---
title: web3_sha3 - Polygon
description: Example code for the web3_sha3 ws method. Сomplete guide on how to use web3_sha3 ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - array of string

the data to convert into a SHA3 hash.

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "web3_sha3",
"params": ["0xf2a2b854721d4372474fc76cc13445a73369c0c334f4935c88bde3c310f28c9a"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xf5d3389b32cee33308ce9af2d8aefa1517aa90ccb7b1d2eb29c61f13e1fd3cea"
}
```

