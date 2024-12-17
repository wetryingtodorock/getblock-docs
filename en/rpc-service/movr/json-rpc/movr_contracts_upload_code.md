---
title: movr:contracts_upload_code \[POST\] {disallowed}
description: Upload new code without instantiating a contract from itNot available in newer versions of the contracts interfaces
---

### Parameters


`uploadRequest` - CodeUploadRequest

None

`at` - BlockHash

optional

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "contracts_upload_code",
"params": [null, null],
"id": "getblock.io"}'
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

