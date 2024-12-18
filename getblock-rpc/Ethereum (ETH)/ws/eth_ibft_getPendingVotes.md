---
title: ibft_getPendingVotes  {disallowed} - Ethereum
description: Example code for the ibft_getPendingVotes  {disallowed} ws method. Сomplete guide on how to use ibft_getPendingVotes  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_getPendingVotes",
"params": [],
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

