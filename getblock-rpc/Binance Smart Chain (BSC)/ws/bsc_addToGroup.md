---
title: addToGroup  {disallowed} - Binance Smart Chain
description: Example code for the addToGroup  {disallowed} ws method. Сomplete guide on how to use addToGroup  {disallowed} ws in GetBlock.io Web3 documentation.

### Parameters


`DATA` - None

60 Bytes - The identity address to add to a group

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "addToGroup",
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

