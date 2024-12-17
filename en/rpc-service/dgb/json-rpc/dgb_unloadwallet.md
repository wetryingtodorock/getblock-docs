---
title: dgb:unloadwallet  {disallowed} - DigiByte
description: Example code for the dgb:unloadwallet  {disallowed} json-rpc method. Сomplete guide on how to use dgb:unloadwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`wallet_name` - string, optional, default=the wallet name from the RPC
endpoint

The name of the wallet to unload. Must be provided in the RPC endpoint
or this parameter (but not both).

`load_on_startup` - boolean, optional, default=null

Save wallet name to persistent settings and load on startup. True to add
wallet to startup list, false to remove, null to leave unchanged.

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "unloadwallet",
"params": [null, null],
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

