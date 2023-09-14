---
title: cro:eth_coinbase \[POST\]
description: Returns the client coinbase address. The coinbase address is the accountto pay mining rewards to.To set a coinbase address, start Besu with the --miner-coinbase optionset to a valid Ethereum account address. You can get the Ethereumaccount address from a client such as MetaMask or Etherscan.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://cro.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "rpc error: code = Unknown desc = validator not found for crcvalcons1vvk5s0mvdtd6r84pd6jxuchk8ry34qhd2lyzk2"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

