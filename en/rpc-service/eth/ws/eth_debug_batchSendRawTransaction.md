---
title: eth:debug_batchSendRawTransaction  {disallowed} - Ethereum
description: Example code for the eth:debug_batchSendRawTransaction  {disallowed} ws method. Сomplete guide on how to use eth:debug_batchSendRawTransaction  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

The signed transaction data array.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_batchSendRawTransaction",
"params": [["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7"]],
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

