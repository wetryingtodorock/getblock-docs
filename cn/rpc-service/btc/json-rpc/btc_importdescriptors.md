---
title: btc:importdescriptors \[POST\] {disallowed}
description: Import descriptors. This will trigger a rescan of the blockchain basedon the earliest timestamp of all descriptors being imported. Requires anew wallet backup.Note This call can take over an hour to complete if using an earlytimestamp during that time, other rpc calls may report that theimported keys, addresses or scripts exist but related transactions arestill missing.
---

### Parameters


`requests` - json array, required

Data to be imported

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "importdescriptors",
"params": [null],
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

