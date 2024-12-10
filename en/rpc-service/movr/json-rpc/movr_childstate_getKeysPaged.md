---
title: movr:childstate_getKeysPaged  {disallowed} - Moonriver
description: Example code for the movr:childstate_getKeysPaged  {disallowed} json-rpc method. Сomplete guide on how to use movr:childstate_getKeysPaged  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`childKey` - PrefixedStorageKey

None

`prefix` - StorageKey

None

`count` - u32

None

`startKey` - StorageKey

None

`at` - Hash

None

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "childstate_getKeysPaged",
"params": [null, null, null, null, null],
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

