---
title: ksm:system_properties \[POST\]
description: Get a custom set of properties as a JSON object, defined in the chainspec.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "system_properties",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "ss58Format": 0,
        "tokenDecimals": 10,
        "tokenSymbol": "ksm"
    }
}
```

