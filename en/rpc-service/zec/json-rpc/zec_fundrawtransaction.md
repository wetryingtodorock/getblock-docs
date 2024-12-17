---
title: zec:fundrawtransaction - Zcash
description: Example code for the zec:fundrawtransaction json-rpc method. Сomplete guide on how to use zec:fundrawtransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hexstring` - string

The hex string of the raw transaction.

`includeWatching` - boolean

Optional, default=false

Also select inputs which are watch only.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "fundrawtransaction",
"params": [null, null],
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

