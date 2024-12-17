---
title: engine_createBlock  {disallowed} - Polkadot
description: Example code for the engine_createBlock  {disallowed} json-rpc method. Сomplete guide on how to use engine_createBlock  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`createEmpty` - bool

None

`finalize` - bool

None

`parentHash` - BlockHash

None

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "engine_createBlock",
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

