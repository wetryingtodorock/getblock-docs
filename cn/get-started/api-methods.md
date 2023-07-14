---
lastUpdated: June 10, 2023
---

# API 方法（JSON-RPC、REST、WebSockets 等）
每個節點都有自己的一套與區塊鍊網絡交互的方法。 您可以在[此處](https://getblock.io/docs/nodes-endpoints/)找到 GetBlock 支持的每個節點的文檔。 選擇所需的節點，然後點擊“API 文檔”部分中提供的方法的鏈接。

例如，您可以獲取有關以太坊網絡中最後一個區塊的信息，如下所示：
<pre>
curl --location --request POST 'https://eth.getblock.io/mainnet/' \
--header 'x-api-key: <YOUR-API-KEY>' \
--header 'Content-Type: application/json' \
--data-raw '{
  "id": "blockNumber",
  "jsonrpc": "2.0",
  "method": "eth_getBlockByNumber",
  "params": ["latest", false]
}'
</pre>
