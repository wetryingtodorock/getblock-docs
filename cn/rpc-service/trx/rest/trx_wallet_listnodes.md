---
title: trx:/wallet/listnodes \[GET\]
description: Query the list of nodes connected to the API node
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/listnodes' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "nodes": [
        {
            "address": {
                "host": "3137302e3138372e3138392e3331",
                "port": 18888
            }
        },
        {
            "address": {
                "host": "35312e38312e3138342e3931",
                "port": 30001
            }
        }
    ]
}
```

