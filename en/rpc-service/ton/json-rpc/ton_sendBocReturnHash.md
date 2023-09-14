---
title: ton:/sendBocReturnHash \[POST\] {disallowed}
description: Send serialized boc file fully packed and serialized external messageto blockchain. The method returns message hash.
---

### Parameters


`boc` - body

string

serialized boc file, b64 encoded bag of cells

### Request

``` java
curl --location --request POST 'https://ton.getblock.io/mainnet/rest//sendBocReturnHash?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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

