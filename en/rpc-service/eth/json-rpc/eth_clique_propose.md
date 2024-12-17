---
title: eth:clique_propose  {disallowed} - Ethereum
description: Example code for the eth:clique_propose  {disallowed} json-rpc method. Сomplete guide on how to use eth:clique_propose  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

20-byte address.

`boolean` - None

true to propose adding signer or false to propose removing signer.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_propose",
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

