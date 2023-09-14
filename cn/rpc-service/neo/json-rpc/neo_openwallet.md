---
title: neo:openwallet \[POST\] {disallowed}
description: Opens the specified wallet file.To be on the safe side this method is disabled by default. If you doneed to use this method you can manually enable this method in theRpcServer configuration file.
---

### Parameters


`path` - string

The wallet file path

`password` - string

In plain text.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "openwallet",
"params": [null, null],
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

