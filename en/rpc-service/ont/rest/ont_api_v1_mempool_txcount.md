---
title: ont:/api/v1/mempool/txcount \[GET\]
description: Fetch current transaction count in the memory pool
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/unboundong/A9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getmempooltxcount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Version": "1.0.0",
    "Result": [
        100,
        50
    ]
}
```

