---
lastUpdated: June 10, 2023
---

# API methods (JSON-RPC, REST, WebSockets, etc.)

Each node has its own set of methods for interaction with the blockchain network. You can find the documentation for each node supported by GetBlock [here](https://getblock.io/docs/nodes-endpoints/). Choose the desired node and press the link with the provided method in the “API Docs” section.

For example, you can get information about the last block in the Ethereum network as follows:
```
curl --location --request POST 'https://eth.getblock.io/mainnet/' \
--header 'x-api-key: <YOUR-API-KEY>' \
--header 'Content-Type: application/json' \
--data-raw '{
  "id": "blockNumber",
  "jsonrpc": "2.0",
  "method": "eth_getBlockByNumber",
  "params": ["latest", false]
}'
```
