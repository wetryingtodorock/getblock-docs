---
title: dgb:preciousblock - DigiByte
description: Example code for the dgb:preciousblock json-rpc method. Сomplete guide on how to use dgb:preciousblock json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockhash` - string, required

the hash of the block to mark as precious

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "preciousblock",
"params": ["8aef53e812659444b72dfa021ccbfddfb795e04889788c8dee802113e186acf3"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": null
}
```

