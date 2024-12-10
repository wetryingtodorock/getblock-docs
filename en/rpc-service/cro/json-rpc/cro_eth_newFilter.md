---
title: cro:eth_newFilter - Cronos
description: Example code for the cro:eth_newFilter json-rpc method. Сomplete guide on how to use cro:eth_newFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

Filter options

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newFilter",
"params": [{"topics": ["0xb7407a6d74c6472bf99c4c9abe0860dc439469421c42c060639733b2309b05c7"]}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xe0b03d6a3ee36af033095d805aa675e2"
}
```

