---
title: zec:z_getpaymentdisclosure \[POST\] {disallowed}
description: Generate a payment disclosure for a given joinsplit output.EXPERIMENTAL FEATUREWARNING z_getpaymentdisclosure is disabled.
---

### Parameters


`txid` - string

None

`js_index` - string

None

`output_index` - string

None

`message` - string

Optional

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_getpaymentdisclosure",
"params": [null, null, null, null],
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

