---
title: trx:/wallet/getbandwidthprices \[GET\]
description: Query historical bandwidth unit price
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/getbandwidthprices' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "prices": "0:10,1606240800000:40,1613044800000:140,1627279200000:1000"
}
```

