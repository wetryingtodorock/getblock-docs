---
title: xem:/account/unlocked/info \[POST\] {disallowed}
description: Each node can allow users to harvest with their delegated key on thatnode. The NIS configuration has entries for configuring the maximumnumber of allowed harvesters and optionally allow harvesting only forcertain account addresses. The unlock info gives information about themaximum number of allowed harvesters and how many harvesters are alreadyusing the node.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://xem.getblock.io/account/unlocked/info' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

