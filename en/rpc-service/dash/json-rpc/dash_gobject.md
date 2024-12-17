---
title: dash:gobject \[POST\] {disallowed}
description: votes on a governance object by all masternodes (using masternode.confsetup).
---

### Parameters


`method name` - string

None

`governance-hash` - string (hex)

Hash of the governance object.

`signal` - string

Vote signal: funding, valid, or delete

`outcome` - string

Vote outcome: yes, no, or abstain

`alias` - string

Alias of voting masternode

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gobject",
"params": ["vote-many", null, null, null, null],
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

