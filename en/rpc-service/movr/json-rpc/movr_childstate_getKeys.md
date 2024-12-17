---
title: movr:childstate_getKeys \[POST\] {disallowed}
description: Returns the keys with prefix from a child storage, leave empty to getall the keys.
---

### Parameters


`childKey` - PrefixedStorageKey

None

`prefix` - StorageKey

None

`at` - Hash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getKeys",
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

