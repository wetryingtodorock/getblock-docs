---
title: apt:/v1/accounts/{account_hash} \[GET\]
description: Gets the authentication key and the sequence number for an accountaddress.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1/accounts/0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "authentication_key": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
    "sequence_number": "497660"
}
```

