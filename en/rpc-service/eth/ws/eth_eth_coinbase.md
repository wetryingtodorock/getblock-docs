---
title: eth:eth_coinbase \[WebSocket\]
description: Returns the client coinbase address. The coinbase address is the accountto pay mining rewards to.To set a coinbase address, start Besu with the --miner-coinbase optionset to a valid Ethereum account address. You can get the Ethereumaccount address from a client such as MetaMask or Etherscan.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "etherbase must be explicitly specified"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

