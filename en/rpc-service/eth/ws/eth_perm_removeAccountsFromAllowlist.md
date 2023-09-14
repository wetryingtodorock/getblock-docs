---
title: eth:perm_removeAccountsFromAllowlist \[WebSocket\] {disallowed}
description: Removes accounts (participants) from the accounts permissions list.
---

### Parameters


`list of strings` - None

List of account addresses.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "perm_removeAccountsFromAllowlist",
"params": [null],
"id": "getblock.io"}
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

