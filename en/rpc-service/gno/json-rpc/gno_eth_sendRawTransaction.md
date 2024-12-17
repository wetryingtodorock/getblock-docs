---
title: gno:eth_sendRawTransaction \[POST\] {disallowed}
description: Sends a signed transaction. A transaction can send ether, deploy acontract, or interact with a contract. Set the maximum transaction feefor transactions using the --rpc-tx-feecap CLI option.You can interact with contracts using eth_sendRawTransaction oreth_call.To avoid exposing your private key, create signed transactions offlineand send the signed transaction data using eth_sendRawTransaction.
---

### Parameters


`data` - hex string

Signed transaction serialized to hexadecimal format.

### Request

``` java
curl --location --request POST 'https://gno.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_sendRawTransaction",
"params": ["0xf869018203e882520894f17f52151ebef6c7334fad080c5704d77216b732881bc16d674ec80000801ba02da1c48b670996dcb1f447ef9ef00b33033c48a4fe938f420bec3e56bfd24071a062e0aa78a81bf0290afbc3a9d8e9a068e6d74caa66c5e0fa8a46deaae96b0833"],
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

