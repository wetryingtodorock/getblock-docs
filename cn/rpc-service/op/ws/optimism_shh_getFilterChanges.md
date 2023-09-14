---
title: optimism:shh_getFilterChanges \[WebSocket\] {disallowed}
description: Polling method for whisper filters. Returns new messages since the lastcall of this method.Note calling the shh_getMessages method, will reset the buffer for thismethod, so that you won’t receive duplicate messages.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_getFilterChanges",
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

