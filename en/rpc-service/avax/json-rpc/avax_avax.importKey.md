---
title: avax:avax.importKey \[POST\] {disallowed}
description: Give a user control over an address by providing the private key thatcontrols the address.
---

### Parameters


`username` - string

user name

`password` - string

user password

`privateKey` - string

private key

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "avax.importKey",
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

