---
title: xem:/chain/score \[GET\]
description: Gets the current score of the block chain. The higher the score, thebetter the chain. During synchronization, nodes try to get the bestblock chain in the network.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/chain/score' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "score": "13da4dda5fb5c4e8bd"
}
```

