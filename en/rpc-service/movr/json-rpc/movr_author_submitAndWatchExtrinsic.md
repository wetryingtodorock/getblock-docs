---
title: movr:author_submitAndWatchExtrinsic \[POST\] {disallowed}
description: Submit and subscribe to watch an extrinsic until unsubscribed
---

### Parameters


`extrinsic` - Extrinsic

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_submitAndWatchExtrinsic",
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

