---
title: priv_distributeRawTransaction  {disallowed} - Ethereum Classic
description: Example code for the priv_distributeRawTransaction  {disallowed} json-rpc method. Сomplete guide on how to use priv_distributeRawTransaction  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Signed RLP-encoded private transaction.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_distributeRawTransaction",
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
