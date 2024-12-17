---
title: xem:/node/boot  {disallowed} - NEM
description: Example code for the xem:/node/boot  {disallowed} rest method. Сomplete guide on how to use xem:/node/boot  {disallowed} rest in GetBlock.io Web3 documentation.
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

