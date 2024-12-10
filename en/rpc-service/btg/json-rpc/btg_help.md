---
title: btg:help - Bitcoin Gold
description: Example code for the btg:help json-rpc method. Сomplete guide on how to use btg:help json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`command` - string, optional, default=all commands

The command to get help on

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
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
    "result": "List all commands, or get help for a specified command."
}
```

