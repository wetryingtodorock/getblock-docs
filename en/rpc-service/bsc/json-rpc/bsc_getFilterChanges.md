---
title: bsc:getFilterChanges \[POST\] {disallowed}
description: Polling method for whisper filters. Returns new messages since the lastcall of this method.Note calling the shh_getMessages method, will reset the buffer for thismethod, so that you wont receive duplicate messages.
---

### Parameters


`QUANTITY` - None

The filter id

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getFilterChanges",
"params": [null],
"id": "getblock.io"}'
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

