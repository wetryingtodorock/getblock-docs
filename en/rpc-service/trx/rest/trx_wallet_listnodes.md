---
title: /wallet/listnodes - TRON
description: Example code for the /wallet/listnodes rest method. Сomplete guide on how to use /wallet/listnodes rest in GetBlock.io Web3 documentation.
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

