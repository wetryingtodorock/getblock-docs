---
title: eth:perm_addAccountsToAllowlist  {disallowed} - Ethereum
description: Example code for the eth:perm_addAccountsToAllowlist  {disallowed} ws method. Сomplete guide on how to use eth:perm_addAccountsToAllowlist  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`list of strings` - None

List of account addresses.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "perm_addAccountsToAllowlist",
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

