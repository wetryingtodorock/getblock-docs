---
title: ksm:state_subscribeStorage  {disallowed} - Kusama
description: Example code for the ksm:state_subscribeStorage  {disallowed} json-rpc method. Сomplete guide on how to use ksm:state_subscribeStorage  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`keys` - Vector of StorageKey

list of storage keys

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_subscribeStorage",
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

