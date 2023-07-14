---
lastUpdated: June 10, 2023
---

# 驗證

您可以使用 API 密鑰進行身份驗證來授權您的連接，就像連接到我們的節點一樣。 請在儀表板中創建一個新的 API 密鑰或使用現有的 API 密鑰。 然後，請將 API 密鑰複製並粘貼到標頭或查詢字符串中。

```
curl https://api.getblock.io/external/webhook/?api_key={YOUR_API_KEY}
```

或者

```
curl https://api.getblock.io/external/webhook/ -H x-api-key:{YOUR_API_KEY}
```
