---
title: xem:/status \[GET\]
description: Determines the status of NIS.The code can be interpreted as follows 0 Unknown status. 1 NIS isstopped. 2 NIS is starting. 3 NIS is running. 4 NIS is booting thelocal node (implies NIS is running). 5 The local node is booted(implies NIS is running). 6 The local node is synchronized (implies NISis running and the local node is booted). 7 NIS local node does not seeany remote NIS node (implies running and booted). 8 NIS is currentlyloading the block chain from the database. In this state NIS cannotserve any requests.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/status' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "code": 6,
    "message": "status",
    "type": 4
}
```

