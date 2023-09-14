---
title: neo:getapplicationlog \[POST\] {disallowed}
description: Returns the contract event information based on the specified txid. Thecontract event information is stored under the ApplicationLogsdirectory.You must install the plugins ApplicationLogs and LevelDBStore before youcan invoke the method.
---

### Parameters


`txid` - string

Transaction ID

`trigger type` - string

Optional. It has the following options:

\- OnPersist

\- PostPersist

\- Application

\- Verification

\- System: OnPersist \| PostPersist

All: OnPersist \| PostPersist \| Verification \| Application

It defaults to All. You can specify a trigger type.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getapplicationlog",
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

