---
title: dash:ping \[POST\] {disallowed}
description: Sends a P2P ping message to all connected nodes to measure ping time.Results are provided by the getpeerinfo RPC pingtime and pingwait fieldsas decimal seconds.The P2P ping message is handled in a queue with all other commands, soit measures processing backlog, not just network ping.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "ping",
"params": [],
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

