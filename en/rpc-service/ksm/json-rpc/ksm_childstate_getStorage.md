---
title: ksm:childstate_getStorage  {disallowed} - Kusama
description: Example code for the ksm:childstate_getStorage  {disallowed} json-rpc method. Сomplete guide on how to use ksm:childstate_getStorage  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
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

