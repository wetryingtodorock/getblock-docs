---
title: dash:loadwallet \[POST\] {disallowed}
description: Loads a wallet from a wallet file or directory. Note that all walletcommand-line options used when starting dashd will be applied to the newwallet (eg -zapwallettxes, upgradewallet, rescan, etc).
---

### Parameters


`Filename` - string

The wallet directory or .dat file. The wallet can be specified as
file/directory basename (which must be located in the walletdir
directory), or as an absolute path to a file/directory.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "loadwallet",
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

