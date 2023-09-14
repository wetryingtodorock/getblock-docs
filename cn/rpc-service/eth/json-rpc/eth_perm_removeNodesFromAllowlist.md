---
title: eth:perm_removeNodesFromAllowlist \[POST\] {disallowed}
description: Removes nodes from the nodes allowlist.
---

### Parameters


`list of strings` - None

List of enode URLs

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "perm_removeNodesFromAllowlist",
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

