---
title: bsc:getFilterChanges \[WebSocket\] {disallowed}
description: Polling method for whisper filters. Returns new messages since the lastcall of this method.Note calling the shh_getMessages method, will reset the buffer for thismethod, so that you wont receive duplicate messages.
---

### Parameters


`QUANTITY` - None

The filter id

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "getFilterChanges",
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

