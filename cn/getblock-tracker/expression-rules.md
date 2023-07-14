---
lastUpdated: June 10, 2023
---

# 表達式規則

## 比較運算符

- ```==``` 等於
- ```!=``` 不等於
- ```<``` 小於
- ```>``` 大於
- ```<=``` 小於或等於
- ```>=``` 大於或等於

## 邏輯運算符

- ```and```
- ```or```

## 數組運算符

- ```contain```
- ```not contain```

## 一般原則

表達式由條件組成。 例如，表達式 ```(transaction_blockNumber == 1 or block_number == 2)``` 由兩個條件組成： ```(transaction_blockNumber == 1)``` 和 ```(block_number == 2)``` 表達式可以包含一個或多個條件。 條件之間必須有邏輯運算符。

邏輯運算符 ```and``` 意味著表達式中的兩個條件都必須為真。 例如，當區塊號 321 將包含 Gas 等於 123 的交易時，表達式 ```(transaction_gas == 123 and block_number == 321)``` 將被視為 true。

邏輯運算符```or```意味著至少有一個條件必須為真。 例如，當區塊號 321 出現在網絡上，或者任何交易中的 Gas 等於 123 時，表達式 ```(transaction_gas == 123 or block_number == 321)``` 將被視為 true。

## 表達式的構成原則

1. 替換與實體名稱等效的前綴。 例如，如果要跟踪區塊號 42，則表達式應為```(block_number == 42)```，對於交易和收據為```(transaction_blockNumber == 42)```和```(receipt_blockNumber == 42)``` 分別。
2. int 或 uint 等變量在表達式中必須不帶引號，如上例所示。 hex20 и hex32 等變量必須用雙引號括起來，例如 ```(transaction_transactionHash == "0x91e44d7d3d8ebb0b5a9e4b0a276c0124281750182dfac5abead8efc752e6246a")```
3. 將表達式括在圓括號內。
