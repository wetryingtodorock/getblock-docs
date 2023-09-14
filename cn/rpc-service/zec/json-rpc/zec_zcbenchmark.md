---
title: zec:zcbenchmark \[POST\] {disallowed}
description: Runs a benchmark of the selected type samplecount times, returning therunning times of each sample.
---

### Parameters


`benchmarktype` - string

type of benchmark

`samplecount` - string

count of samples to run.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "zcbenchmark",
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

