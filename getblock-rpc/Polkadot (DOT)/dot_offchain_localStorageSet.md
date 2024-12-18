---
title: offchain_localStorageSet  {disallowed} - Polkadot
description: Example code for the offchain_localStorageSet  {disallowed} json-rpc method. Сomplete guide on how to use offchain_localStorageSet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`kind` - StorageKind

None

`key` - Bytes

None

`value` - Bytes

None

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "offchain_localStorageSet",
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

