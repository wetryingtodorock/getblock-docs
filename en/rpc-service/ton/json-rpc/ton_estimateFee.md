---
title: ton:/estimateFee \[POST\] {disallowed}
description: Estimate fees required for query processing. body, init-code andinit-data accepted in serialized format (b64-encoded).
---

### Parameters


`address` - body

string, required

address in any format

`body` - body

string, required

b64-encoded cell with message body

`init_code` - body

string, optional

b64-encoded boc-serialized cell with init-code

`init_data` - body

string, optional

b64-encoded boc-serialized cell with init-data

`ignore_chksig` - body

boolean, optional, default true

If true during test query processing assume that all chksig operations
return True

### Request

``` java
curl --location --request POST 'https://ton.getblock.io/mainnet/rest//estimateFee?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"address": "EQA-kuB9yN9P7LJJ9WAPx1KdPoSKWfO2vzb9itId1_l_Dr4H"}'
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

