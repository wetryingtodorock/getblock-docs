---
title: trx:/wallet/generateaddress \[GET\] {disallowed}
description: Generates a random private key and address pair. Returns a private key,the corresponding address in hex, and base58. There is a security risk.This interface service has been shutdown by the Trongrid. Please use theoffline mode or the node deployed by yourself.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/generateaddress?' \
--header 'x-api-key: YOUR-API-KEY' \
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

