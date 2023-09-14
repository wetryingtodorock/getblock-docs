---
title: btc:mempool \[GET\]
description: Returns various information about the TX mempool. Only supports JSON as output format. Refer to the getmempoolinfo RPC for documentation of the fields.
---

### Example

`GET /rest/mempool/info.json`

### Request

``` java
curl --location --request GET 'https://btc.getblock.io/rest/mempool/info.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
    "loaded": true,
    "size": 119074, 
    "bytes": 79930801, 
    "usage": 299999008, 
    "maxmempool": 300000000, 
    "mempoolminfee": 0.00020734,
    "minrelaytxfee": 0.00001000,
    "unbroadcastcount": 0
}
```
