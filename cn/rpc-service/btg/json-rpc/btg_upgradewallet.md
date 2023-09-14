---
title: btg:upgradewallet \[POST\] {disallowed}
description: Upgrade the wallet. Upgrades to the latest version if no version numberis specified.New keys may be generated and a new wallet backup will need to be made.
---

### Parameters


`version` - numeric, optional, default=169900

The version number to upgrade to. Default is the latest wallet version.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "upgradewallet",
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

