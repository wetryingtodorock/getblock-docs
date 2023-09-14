---
title: xlm:/accounts/{account_id}/data/{key} \[GET\] {disallowed}
description: This endpoint represents a single data for a given account.
---

### Parameters


`account_id` - path

This account's public key encoded in a base32 string representation.

`key` - path

The key name for this data.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/data/datakey' 
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

