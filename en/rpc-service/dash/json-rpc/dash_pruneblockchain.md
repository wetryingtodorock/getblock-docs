---
title: dash:pruneblockchain  {disallowed} - Dash
description: Example code for the dash:pruneblockchain  {disallowed} json-rpc method. Сomplete guide on how to use dash:pruneblockchain  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`height` - number (int)

The block height to prune up to. May be set to a particular height, or a
unix timestamp to prune blocks whose block time is at least 2 hours
older than the provided timestamp.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "pruneblockchain",
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

