---
title: dgb:validateaddress \[POST\]
description: Return information about the given btc address.
---

### Parameters


`address` - string, required

The btc address to validate

### Request

``` java
curl --location --request POST 'https://dgb.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "validateaddress",
"params": ["bc1q09vm5lfy0j5reeulh4x5752q25uqqvz34hufdl"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "isvalid": false
    }
}
```

