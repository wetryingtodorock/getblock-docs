---
title: zec:help \[POST\]
description: List all commands, or get help for a specified command.
---

### Parameters


`command` - string

Optional.

The command to get help on.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "help",
"params": ["help"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "help ( \"command\" )  List all commands, or get help for a specified command."
}
```

