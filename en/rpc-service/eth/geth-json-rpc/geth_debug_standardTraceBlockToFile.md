---
title: geth:debug_standardTraceBlockToFile \[POST\] {disallowed}
description: It streams output to disk during the execution, to not blow up thememory usage on the nodeThis means that this method is only ‘useful’ for callers who control thenode – at least sufficiently to be able to read the artefacts from thefilesystem after the fact.
---

### Parameters


`hash` - string

block hash

`tx` - json object

transaction hash

disableMemory - use memory of not

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBlockToFile",
"params": ["0x0003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700", {"0x263cdd926f7a8e72a3c3186f093200b3a39b7376e3ef845f66a3672e931ded3d", false]},
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

