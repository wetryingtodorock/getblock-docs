---
title: eth_newFilter - Ethereum
description: Example code for the eth_newFilter json-rpc method. Сomplete guide on how to use eth_newFilter json-rpc in GetBlock.io Web3 documentation.
---

### Parameters

A `filter object` with the fillowing keys and their values:

- `address`: [optional] A contract address or a list of addresses from which logs should originate.
- `fromBlock`: [optional, default is latest] A hexadecimal block number, or the string latest, earliest or pending.
- `toBlock`: [optional, default is latest] A hexadecimal block number, or the string latest, earliest or pending.
- `topics`: [optional] An array of 32 bytes DATA topics. Topics are order-dependent.

### Specifying topic filters

Topics are order-dependent. A transaction with a log with topics [A, B] will be matched by the following topic filters:

- `[]`: Anything.
- `[A]`: A in the first position, and anything after.
- `[null, B]`: Anything in first position AND B in second position, and anything after.
- `[A, B]`: A in the first position AND B in second position, and anything after.
- `[[A, B], [A, B]]`: (A OR B) in first position AND (A OR B) in second position, and anything after.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
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
    "result": "0x7087a9a20c62b41cd0290a6e6a9e0e33"
}
```

