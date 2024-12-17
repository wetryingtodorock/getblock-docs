---
title: sol:getTransaction - Solana
description: Example code for the sol:getTransaction json-rpc method. Сomplete guide on how to use sol:getTransaction json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`signature` - string

transaction signature as base-58 encoded string

`Config` - object

Configuration object containing the following optional fields: -
encoding: string (optional) - encoding for each returned Transaction,
either "json", "jsonParsed", "base58" (slow), "base64". If parameter not
provided, the default encoding is "json". "jsonParsed" encoding attempts
to use program-specific instruction parsers to return more
human-readable and explicit data in the transaction.message.instructions
list. If "jsonParsed" is requested but a parser cannot be found, the
instruction falls back to regular JSON encoding (accounts, data, and
programIdIndex fields). - commitment (optional) - "processed" is not
supported. If parameter not provided, the default is "finalized".

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getTransaction",
"params": ["2nBhEBYYvfaAe16UMNqRHre4YNSskvuYgx3M6E4JP1oDYvZEJHvoPzyUidNgNX5r9sTyN1J9UxtbCXy2rqYcuyuv", "json"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

