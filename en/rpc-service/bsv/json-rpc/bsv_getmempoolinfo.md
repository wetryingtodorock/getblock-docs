---
title: bsv:getmempoolinfo - Bitcoin SV
description: Example code for the bsv:getmempoolinfo json-rpc method. Сomplete guide on how to use bsv:getmempoolinfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getmempoolinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "bytes": 1738267,
        "loaded": true,
        "maxmempool": 300000000,
        "mempoolminfee": 1e-05,
        "minrelaytxfee": 1e-05,
        "size": 6478,
        "usage": 7952928
    }
}
```

