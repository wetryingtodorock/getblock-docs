---
title: dgb:generateblock  {disallowed} - DigiByte
description: Example code for the dgb:generateblock  {disallowed} json-rpc method. Сomplete guide on how to use dgb:generateblock  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`output` - string, required

The address or descriptor to send the newly generated btc to.

`transactions` - json array, required

An array of hex strings which are either txids or raw transactions.

Txids must reference transactions currently in the mempool.

All transactions must be valid and in valid order, otherwise the block
will be rejected.

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/msinnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "generateblock",
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

