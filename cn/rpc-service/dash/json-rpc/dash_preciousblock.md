---
title: dash:preciousblock \[POST\]
description: Treats a block as if it were received before others with the same work.A later preciousblock call can override the effect of an earlier one.The effects of preciousblock are not retained across restarts.
---

### Parameters


`header hash` - string (hex)

The hash of the block to mark as precious.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "preciousblock",
"params": ["00000000000000093711aeacfe1a827cb43c6d626230cdd2e41ad6f43c1e79d3"],
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

