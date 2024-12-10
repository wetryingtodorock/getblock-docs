---
title: etc:clique_discard  {disallowed} - Ethereum Classic
description: Example code for the etc:clique_discard  {disallowed} json-rpc method. Сomplete guide on how to use etc:clique_discard  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

20-byte address of proposed signer.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "clique_discard",
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

