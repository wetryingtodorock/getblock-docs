---
title: listreceivedbyaccount  {disallowed} - Zcash
description: Example code for the listreceivedbyaccount  {disallowed} json-rpc method. Сomplete guide on how to use listreceivedbyaccount  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`minconf` - numeric

Optional, default=1

The minimum number of confirmations before payments are included.

`includeempty` - boolean

Optional, default=false

Whether to include accounts that haven't received any payments.

`includeWatchonly` - boolean

Optional, default=false

Whether to include watchonly addresses.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "listreceivedbyaccount",
"params": [null, null, null],
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

