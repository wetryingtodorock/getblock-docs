---
title: dash:disconnectnode \[POST\] {disallowed}
description: Immediately disconnects from a specified node.
---

### Parameters


`address` - string

The node you want to disconnect from as a string in the form of
IP_address:port.

Updated in Bitcoin Core 0.14.1

`nodeid` - number

Optional.

The node ID (see getpeerinfo for node IDs)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "disconnectnode",
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

