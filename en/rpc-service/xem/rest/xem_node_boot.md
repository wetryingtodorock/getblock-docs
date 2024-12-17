---
title: xem:/node/boot \[POST\] {disallowed}
description: Boots the local node and thus assign an account (the identity) to thelocal node.
---

### Parameters


`bootNodeRequest` -

A BootNodeRequest JSON object. The BootNodeRequest JSNON object is used
to transfer the relevant data for booting a local node to NIS. With the
boot data NIS can create the local node object and connect to the
network.

### Request

``` java
curl --location --request POST 'https://xem.getblock.io/node/boot' 
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

