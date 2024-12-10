---
title: dash:quorum_memberof  {disallowed} - Dash
description: Example code for the dash:quorum_memberof  {disallowed} json-rpc method. Сomplete guide on how to use dash:quorum_memberof  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`submethod` - string

None

`proTxHash` - string

ProTxHash of the masternode.

`scanQuorumsCount` - number

Optional.

Number of quorums to scan for. If not specified, the active quorum count
for each specific quorum type is used.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "quorum",
"params": ["memberof", null, null],
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

