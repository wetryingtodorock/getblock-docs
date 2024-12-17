---
title: dot:childstate_getStorage \[POST\] {disallowed}
description: Returns a child storage entry at a specific block state
---

### Parameters


`childKey` - PrefixedStorageKey

None

`key` - StorageKey

None

`at` - Hash

None

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getStorage",
"params": [null, null, null],
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

