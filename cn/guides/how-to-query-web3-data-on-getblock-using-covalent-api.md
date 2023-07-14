---
lastUpdated: June 10, 2023
---

# 如何使用 Covalent API 查詢 GetBlock 上的 web3 數據

Covalent 很高興與 GetBlock 等行業領先的服務提供商合作。 Covalent 提供統一的 API 來釋放十億種可能性，並為所有區塊鍊網絡中的資產帶來完全的透明度和可見性。 簡而言之，該 API 允許您無需代碼即可從多個區塊鏈中提取詳細、粒度和歷史的區塊鏈交易數據。 Covalent API 允許您創建全新的應用程序或增強現有應用程序，而無需配置或維護基礎設施。

## 需要 API 密鑰

在 [https://www.covalenthq.com/platform/](https://www.covalenthq.com/platform/) 註冊以獲取您的 API 密鑰

## API 文檔

Covalent API 文檔參考 ([https://www.covalenthq.com/docs/api](https://www.covalenthq.com/docs/api)) 提供了有關受支持的區塊鍊網絡、可用 API 端點的所有詳細信息 ，甚至使用戶能夠直接從瀏覽器發出所有 API 請求。

關於共價 API 需要注意的要點是：

- 共價 API 是 RESTful 的；
- 共價 API 密鑰必須作為查詢參數傳遞給所有請求，使用：key=API_KEY；
- 所有端點默認返回格式為JSON，部分端點支持CSV格式；
- 刷新率分類為：<br/>
  實時：30秒或2個區塊；<br/>
  批量：10m或40塊；
- 在區塊鍊網絡之間切換的主要查詢參數是 chain_id。 例如，要獲取以太坊和幣安智能鏈上錢包地址的所有代幣餘額（包括 NFT），需要向balances_v2端點發出請求：

https://api.covalenthq.com/v1/{chain_id}/address/{address}/balances_v2/

其中，以太坊主網的 chain_id 為 1，BSC 主網的 chain_id 為 56。
Covalent API 支持所有主要的區塊鍊網絡。 有關包括 chain_id 值的完整列表，請參閱 [https://www.covalenthq.com/docs/networks](https://www.covalenthq.com/docs/networks/?utm_source=website&utm_medium=info&utm_campaign=getblock)。

## 學習資源：

Covalent 以教程、操作指南和案例研究的形式提供全面的學習資源，網址為 [https://www.covalenthq.com/docs/learn](https://www.covalenthq.com/docs/learn/ ?utm_source=網站&utm_medium=信息&utm_campaign=getblock)

## 用例：

訪問豐富的歷史區塊鏈數據可以解鎖大量用例，其中許多用例仍然未知，並且隨著該領域創新的快速步伐而逐漸浮出水面。 當前的一些用例包括：

- 多鏈錢包顯示余額、交易、投資回報率、投資組合價值以及代幣集中度、數量和分佈的分析
- NFT 儀表板顯示收藏品的價格趨勢、流動性和投資回報率
- 稅務合規工具
- DEX 分析和透明度儀表板
- DAO 治理和分析儀表板
  要了解開發人員使用 Covalent API 構建的內容，請查看我們的項目展示：[https://www.covalenthq.com/docs/project-showcase](https://www.covalenthq.com/docs/project-showcase /?utm_source=網站&utm_medium=info&utm_campaign=getblock)

## 開發者工具：

這些工具是對 Covalent API 的補充，並提供額外的特性和功能來提取和分析複雜的區塊鏈數據。 下面的頁面列出了社區構建的為 Covalent API 用戶提供價值的工具。

注意：這些工具不是由共價團隊維護的，用戶在項目中使用這些工具之前應自行進行盡職調查來評估這些工具。
[https://www.covalenthq.com/docs/tools/community](https://www.covalenthq.com/docs/tools/community/?utm_source=website&utm_medium=info&utm_campaign=getblock)
