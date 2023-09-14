---
title: dot:childstate_getStorageEntries \[POST\] {disallowed}
description: Returns child storage entries for multiple keys at a specific blockstate
---

### Parameters


`childKey` - PrefixedStorageKey

None

`keys` - list of StorageKey

None

`at` - hash

optional

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getStorageEntries",
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

