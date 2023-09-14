---
title: dash:getgovernanceinfo \[POST\]
description: Returns an object containing governance parameters.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getgovernanceinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "governanceminquorum": 10,
        "lastsuperblock": 1528672,
        "nextsuperblock": 1545288,
        "proposalfee": 5.0,
        "superblockcycle": 16616
    }
}
```

