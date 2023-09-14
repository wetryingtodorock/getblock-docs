---
title: btg:disconnectnode \[POST\] {disallowed}
description: Immediately disconnects from the specified peer node.Strictly one out of ‘address’ and ‘nodeid’ can be provided to identifythe node.To disconnect by nodeid, either set ‘address’ to the empty string, orcall using the named ‘nodeid’ argument only.
---

### Parameters


`address` - string, optional, default=fallback to nodeid

The IP address/port of the node

`nodeid` - numeric, optional, default=fallback to address

The node ID (see getpeerinfo for node IDs)

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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

