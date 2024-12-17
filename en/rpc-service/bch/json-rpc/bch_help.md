---
title: bch:help \[POST\]
description: List all commands, or get help for a specified command.
---

### Parameters


`command` - string, optional, default=all commands

The command to get help on

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "help",
"params": ["logging"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "logging. Gets and sets the logging configuration",
    "error": null,
    "id": "getblock.io"
}
```

