---
title: mempool - Bitcoin
description: Example code for the mempool rest method. Сomplete guide on how to use mempool rest in GetBlock.io Web3 documentation.
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
