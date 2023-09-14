---
title: dash:getmemoryinfo \[POST\] {disallowed}
description: Returns information about memory usage.
---

### Parameters


`mode` - string

Optional. Default = stats

Added in Dash Core 0.15.0

Determines what kind of information is returned.

\- stats returns general statistics about memory usage in the daemon.

\- mallocinfo returns an XML string describing low-level heap state
(only available if compiled with glibc 2.10+).

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmemoryinfo",
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

