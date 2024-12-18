---
title: admin_removePeer  {disallowed} - Ethereum
description: Example code for the admin_removePeer  {disallowed} json-rpc method. Сomplete guide on how to use admin_removePeer  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`string` - None

Enode URL of peer to remove.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_removePeer",
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

