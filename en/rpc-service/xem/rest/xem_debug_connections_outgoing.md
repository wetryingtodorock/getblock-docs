---
title: xem:/debug/connections/outgoing \[GET\]
description: Gets an audit collection of outgoing calls. You can monitor theoutstanding and recent outgoing requests with this information.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/debug/connections/outgoing' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "most-recent": [
        {
            "elapsed-time": 2,
            "host": "xem44.allnodes.me",
            "id": 1392509,
            "path": "/transactions/unconfirmed",
            "start-time": 238620183
        },
        {
            "elapsed-time": 2,
            "host": "xem44.allnodes.me",
            "id": 1392508,
            "path": "/chain/score",
            "start-time": 238620183
        },
        {
            "elapsed-time": 6,
            "host": "108.61.168.86",
            "id": 1392507,
            "path": "/transactions/unconfirmed",
            "start-time": 238620179
        }
    ]
}
```

