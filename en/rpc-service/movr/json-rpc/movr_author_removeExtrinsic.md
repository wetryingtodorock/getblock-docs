---
title: movr:author_removeExtrinsic \[POST\] {disallowed}
description: Remove given extrinsic from the pool and temporarily ban it to preventreimporting
---

### Parameters


`bytesOrHash` - Vector of ExtrinsicOrHash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_removeExtrinsic",
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

