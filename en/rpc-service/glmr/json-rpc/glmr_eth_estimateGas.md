---
title: glmr:eth_estimateGas - Moonbeam
description: Example code for the glmr:eth_estimateGas json-rpc method. Сomplete guide on how to use glmr:eth_estimateGas json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`object` - json object

The transacion call object in format: { "from": "address" (optional,
string) - The address the transaction is sent from. "to": "address"
(optional, string) - The address the transaction is directed to. "gas":
"quantity" (optional, string) - Integer of the gas provided for the
transaction execution. eth_call consumes zero gas, but this parameter
may be needed by some executions. "gasPrice": "quantity" (optional,
string) - Integer of the gasPrice used for each paid gas "value":
"quantity" (optional, string) - Integer of the value sent with this
transaction "data": "data" (optional, string) - Hash of the method
signature and encoded parameters. }

### Request

``` java
curl --location --request POST 'https://glmr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_estimateGas",
"params": [{"from": "0xb60e8dd61c5d32be8058bb8eb970870f07233155", "to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567", "gas": "0x76c0", "gasPrice": "0x9184e72a000", "value": "0x9184e72a", "data": "0xd46e8dd67c5d32be8d46e8dd67c5d32be8058bb8eb970870f072445675058bb8eb970870f072445675"}],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32603,
        "message": "insufficient funds for transfer"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

