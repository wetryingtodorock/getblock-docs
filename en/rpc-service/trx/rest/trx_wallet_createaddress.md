---
title: trx:/wallet/createaddress \[POST\] {disallowed}
description: Create address from a specified password string (NOT PRIVATE KEY). Thereis a security risk. This interface service has been shutdown by theTrongrid. Please use the offline mode or the node deployed by yourself.
---

### Parameters


`value` - string, required

value is the password, converted from ascii to hex. i.e. the pass
phrase.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createaddress' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
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

