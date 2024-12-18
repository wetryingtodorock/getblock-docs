---
title: gobject_vote-many  {disallowed} - Dash
description: Example code for the gobject_vote-many  {disallowed} json-rpc method. Сomplete guide on how to use gobject_vote-many  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

