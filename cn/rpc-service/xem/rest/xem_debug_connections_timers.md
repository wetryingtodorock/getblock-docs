---
title: xem:/debug/connections/timers \[GET\]
description: Gets an array of task monitor structures. You can monitor the statisticsfor periodic tasks with this information.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/debug/connections/timers' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "data": [
        {
            "last-delay-time": 3000,
            "executions": 1024,
            "failures": 0,
            "successes": 1024,
            "last-operation-start-time": 9317695,
            "is-executing": 0,
            "name": "FORAGING",
            "average-operation-time": 0,
            "last-operation-time": 0
        },
        {
            "last-delay-time": 74181,
            "executions": 71,
            "failures": 0,
            "successes": 71,
            "last-operation-start-time": 9317654,
            "is-executing": 0,
            "name": "REFRESH",
            "average-operation-time": 6,
            "last-operation-time": 7
        }
    ]
}
```

