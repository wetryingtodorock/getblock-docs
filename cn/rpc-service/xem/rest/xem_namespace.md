---
title: xem:/namespace \[GET\]
description: Gets the namespace with given id.
---

### Parameters


`namespace` -

The namespace id.

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/namespace?namespace=cactus'  
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "fqn": "cactus",
    "height": 3915451,
    "owner": "NDOQZVUH5ZZHPFOFFIF3QYIDU2CRVZOAH5DAOCF6"
}
```

