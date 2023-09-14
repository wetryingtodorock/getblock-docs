---
title: neo:sendmany \[POST\] {disallowed}
description: Bulk transfer order, and you can specify a change address.Before you can invoke this method you must call the RPC methodopenwallet to open the wallet first.
---

### Parameters


`from` - string

Optional. The address from which you transfer the asset.

`outputs_array` - array

Array, the data structure of each element in the array is as follows:

{"asset": asset,"value": value,"address": address, "signers": signers}

\- asset : Asset ID (asset identifier), the NEP-17 contract scripthash

\- value : Transfer amount

\- address : Destination address

\- signers : The signature account of transaction

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "sendmany",
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

