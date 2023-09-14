---
title: btg:ping \[POST\] {disallowed}
description: Requests that a ping be sent to all other nodes, to measure ping time.Results provided in getpeerinfo, pingtime and pingwait fields aredecimal seconds.Ping command is handled in queue with all other commands, so it measuresprocessing backlog, not just network ping.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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

