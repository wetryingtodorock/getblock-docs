---
title: dash:/mempool/info.json \[GET\]
description: The GET mempool/info operation returns information about the node’scurrent transaction memory pool. Supports only json as output format.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/mempool/info.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "bytes": 10292,
    "instantsendlocks": 29,
    "loaded": true,
    "maxmempool": 300000000,
    "mempoolminfee": 1e-05,
    "minrelaytxfee": 1e-05,
    "size": 30,
    "usage": 39808
}
```

