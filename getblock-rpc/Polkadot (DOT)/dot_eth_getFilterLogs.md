---
title: eth_getFilterLogs  {disallowed} - Polkadot
description: Example code for the eth_getFilterLogs  {disallowed} json-rpc method. Сomplete guide on how to use eth_getFilterLogs  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`index` - U256

None

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getFilterLogs",
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
