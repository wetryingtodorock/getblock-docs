---
title: dot:state_call  {disallowed} - Polkadot
description: Example code for the dot:state_call  {disallowed} json-rpc method. Сomplete guide on how to use dot:state_call  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`method` - Text

method to call

`data` - Bytes

data

`at` - BlockHash

block hash

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "state_call",
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

