---
lastUpdated: October 24, 2023
---

# 使用訪問令牌進行身份驗證

建立帳戶並登入後，您將被引導至 GetBlock 儀表板。

![screenshot 1](https://storage.getblock.io/web/docs/get-started/auth-with-access-token/screenshot_1.webp)

從這裡，您可以設定端點來存取任何支援的區塊鏈。 只需選擇協定、網路和 API 介面/插件即可。

所有端點都遵循相同的格式：

```https://go.getblock.io/<ACCESS_TOKEN>/```

注意：確保將 <ACCESS_TOKEN> 替換為從 GetBlock 儀表板收到的特定存取權杖。

要發出請求，只需使用此完整端點即可。 您的授權是透過端點路徑中存在的存取權杖來實現的。 該令牌還包含重要的路線資訊。

注意：訪問令牌不能在標頭中發送。

