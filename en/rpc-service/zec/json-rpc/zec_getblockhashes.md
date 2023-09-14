---
title: zec:getblockhashes \[POST\] {disallowed}
description: Returns array of hashes of blocks within the timestamp range provided,greater or equal to low, less than high.WARNING getblockhashes is disabled.
---

### Parameters


`high.` - numeric

The newer block timestamp.

`low` - numeric

The older block timestamp.

`options` - string

Optional.

A json object:

{

"noOrphans": true\|false (boolean) will only include blocks on the main
chain

"logicalTimes": true\|false (boolean) will include logical timestamps
with hashes

}

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblockhashes",
"params": [null, null, null],
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

