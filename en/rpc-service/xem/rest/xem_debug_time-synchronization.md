---
title: xem:/debug/time-synchronization \[GET\]
description: Gets an array of time synchronization results. You can monitor thechange in network time with this information.A time synchronization result is the outcome of the network timesynchronization of a node with other remote nodes. To agree upon acommon time nodes need to synchronize time every hour.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/debug/time-synchronization' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "data": [
        {
            "change": 0,
            "currentTimeOffset": -8509,
            "dateTime": "2022-10-07 10:06:24"
        },
        {
            "change": 0,
            "currentTimeOffset": -8509,
            "dateTime": "2022-10-07 13:06:34"
        },
        {
            "change": 0,
            "currentTimeOffset": -8509,
            "dateTime": "2022-10-07 16:06:41"
        }
    ]
}
```

