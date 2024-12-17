---
title: xem:/account/status \[GET\]
description: Gets the AccountMetaData from an account. The account meta datadescribes additional information for the account.
---

### Parameters


`address` -

The address of the account.

### Request

``` java
curl --location --request GET 'https://xem.getblock.io/account/status?address=NCXIQA4FF5JB6AMQ53NQ3ZMRD3X3PJEWDJJJIGHT'
 --header 'x-api-key: YOUR-API-KEY' 
 --header 'Content-Type: application/json'
```

###  Response

``` java
{
    "cosignatories": [],
    "cosignatoryOf": [],
    "remoteStatus": "ACTIVE",
    "status": "LOCKED"
}
```

