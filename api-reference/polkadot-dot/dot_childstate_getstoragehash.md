---
title: childstate_getStorageHash  {disallowed} - Polkadot
description: Example code for the childstate_getStorageHash  {disallowed} json-rpc method. Сomplete guide on how to use childstate_getStorageHash  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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
"method": "childstate_getStorageHash",
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
