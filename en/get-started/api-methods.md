---
lastUpdated: October 23, 2023
title: API methods (JSON-RPC, REST, WebSockets, etc.)
description: Choose the appropriate protocol and follow the provided documentation per node to leverage the full capabilities of the GetBlock APIs.
---

# API methods (JSON-RPC, REST, WebSockets, etc.)

Each node has its own set of methods for interaction with the blockchain network. You can find the documentation for each node supported by GetBlock [here](https://getblock.io/docs/nodes-endpoints/). Choose the desired node and press the link with the provided method in the “API Docs” section.

For example, you can get information about the last block in the Ethereum network as follows:
```
curl --location --request POST 'https://go.getblock.io/<ACCESS_TOKEN>/' \
--header 'Content-Type: application/json' \
--data-raw '{
  "id": "blockNumber",
  "jsonrpc": "2.0",
  "method": "eth_getBlockByNumber",
  "params": ["latest", false]
}'
```
