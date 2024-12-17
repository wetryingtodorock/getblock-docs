---
title: xem:/debug/connections/incoming - NEM
description: Example code for the xem:/debug/connections/incoming rest method. Сomplete guide on how to use xem:/debug/connections/incoming rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/debug/connections/incoming' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "most-recent": [
        {
            "elapsed-time": 0,
            "host": "172.20.0.1",
            "id": 79,
            "path": "/debug/connections/incoming",
            "start-time": 238620185
        },
        {
            "elapsed-time": 0,
            "host": "172.20.0.1",
            "id": 78,
            "path": "/debug/time-synchronization",
            "start-time": 238620185
        },
        {
            "elapsed-time": 189098,
            "host": "172.20.0.1",
            "id": 77,
            "path": "/account/transfers/incoming",
            "start-time": 238431087
        }
    ]
}
```

