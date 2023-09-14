---
title: ton:/sendQuery \[POST\] {disallowed}
description: Send query - unpacked external message. This method takes address, bodyand init-params (if any), packs it to external message and sends tonetwork. All params should be boc-serialized.
---

### Parameters


`address` - body

string, required

address in any format

`body` - body

string, required

b64-encoded boc-serialized cell with message body

`init_code` - body

string, optional

b64-encoded boc-serialized cell with init-code

`init_data` - body

string, optional

b64-encoded boc-serialized cell with init-data

### Request

``` java
curl --location --request POST 'https://ton.getblock.io/mainnet/rest//sendQuery?' 
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

