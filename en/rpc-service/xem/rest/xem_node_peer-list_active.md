---
title: xem:/node/peer-list/active - NEM
description: Example code for the xem:/node/peer-list/active rest method. Сomplete guide on how to use xem:/node/peer-list/active rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/node/peer-list/active' 
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "data": [
        {
            "endpoint": {
                "host": "104.238.161.61",
                "port": 7890,
                "protocol": "http"
            },
            "identity": {
                "name": "Hi, I am Alice7",
                "public-key": "64f0c867c52e8d3f7fe478854dbb197646d06041cc16b56595c03a217af6564b"
            },
            "metaData": {
                "application": null,
                "features": 1,
                "networkId": 104,
                "platform": "Oracle Corporation (1.8.0_144) on Linux",
                "version": "0.6.100"
            }
        },
        {
            "endpoint": {
                "host": "162.55.15.6",
                "port": 7890,
                "protocol": "http"
            },
            "identity": {
                "name": "Hi, I am Huge Alice",
                "public-key": "35ee63ac6c4bbf1cb56eeaf5ce4edc591ab0c27e1598672d7915af2333224ece"
            },
            "metaData": {
                "application": null,
                "features": 3,
                "networkId": 104,
                "platform": "Red Hat, Inc. (1.8.0_275) on Linux",
                "version": "0.6.100"
            }
        }
    ]
}
```

