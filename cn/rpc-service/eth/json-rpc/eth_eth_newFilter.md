---
title: eth:eth_newFilter \[POST\]
description: 根據給定的過濾器選項建立過濾器對象，以在狀態變更（日誌）時發出通知。 若要檢查狀態是否已更改，請呼叫 eth_getFilterChanges。
---

### Parameters

具有以下鍵及其值的“過濾器物件”：

- `address`：[可選] 合約位址或日誌應源自的位址清單。
- `fromBlock`: [可選，預設為最新] 十六進位區塊號，或字串最新、最早或待定。
- `toBlock`: [可選，預設為最新] 十六進位區塊號，或字串最新、最早或待定。
- `topics`：[可選] 32 位元組 DATA 主題的陣列。 主題與順序相關。

### 指定主題篩選器

主題與順序相關。 具有主題 [A, B] 的日誌的事務將由以下主題過濾器匹配：

- `[]`：任何東西。
- `[A]`：第一個位置是 A，後面是所有內容。
- `[null, B]`：第一個位置的任何內容和第二個位置的 B 以及之後的任何內容。
- `[A, B]`：A 在第一個位置，B 在第二個位置，以及之後的任何內容。
- `[[A, B], [A, B]]`：（A OR B）在第一個位置並且（A OR B）在第二個位置，以及之後的任何內容。

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

