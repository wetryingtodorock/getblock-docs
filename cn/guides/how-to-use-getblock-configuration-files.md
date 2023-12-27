---
lastUpdated: October 23, 2023
---

# 如何使用GetBlock設定文件

## 如何使用 JSON 設定檔透過curl 發出 HTTP 請求

當您需要存取各種節點端點而無需在程式碼中硬編碼 API 金鑰時，將 GetBlock 的 JSON 設定檔與 curl 結合使用特別有用：

1. 從您的 GetBlock 帳號下載 ```getblock.config.json``` 檔案；
2. 確保您已安裝[jq](https://jqlang.github.io/jq/download/)。 jq 是一個多功能的命令列工具，可以從 JSON 檔案中提取值； 
3. 導覽至已匯入 ```getblock.config.json``` 檔案的工作區或目錄並開啟終端機；
4. 現在，您可以使用curl指令向選取的節點端點發出GET請求：

```
curl -X GET https://go.getblock.io/"$(jq -r '.shared.btc.mainnet.rest[0]' getblock.config.json)"/rest/chaininfo.json
```

## 如何將 GetBlock 的 JavaScript 設定與 Web3.js 結合使用

在本簡短指南中，我們將引導您完成使用 web3.js 和 GetBlock 的 JS 設定檔連接到以太坊節點以及其他 EVM 相容網路的過程。 這種方法抽象化了 API 端點的詳細信息，提供了更高層級的安全性。

1. 確保 web3.js 庫已新增到您的專案中。 為此，請使用以下方法之一：

- Npm: ```npm install web3```
- Yarn: ```yarn add web3```
- 純js連結: ```dist/web3.min.js```

2. 安裝在您的 GetBlock 帳戶中找到的 ```getblock.config.js``` 檔案。 將此文件新增至您的專案目錄；
3. 將 getblock 模組匯入到配置新 Web3 實例的 .js 檔案：

```javascript
const { getblock } = require('./getblock.config.js');
```

4. 連接到以太坊節點並開始使用 web3.js 透過 HTTP 或 WebSocket 發送 API 呼叫，格式如下：

```javascript
const { getblock } = require('./getblock.config.js');
var Web3 = require('web3');

// Create the JSON-RPC provider
var web3Rpc = new Web3(new Web3.providers.HttpProvider(
        getblock.shared.eth.mainnet.rpc[0].go()
));

// Create the WebSocket provider
var web3Ws = new Web3.providers.WebsocketProvider(
        `wss://go.getblock.io/${getblock.shared.eth.mainnet.ws[0].token()}`
));
```

使用 *go()* 方法存取整個端點或使用 *token()* 取得令牌。

## 如何將 JS 配置與 Hardhat 一起使用

GetBlock 的設定檔提供了一種更有組織、更靈活的方法來與以太坊節點和 EVM 相容網路進行交互，而無需在程式碼中暴露敏感的 API 金鑰或憑證。 請依照下列步驟在 Hardhat 中設定 GetBlock 的 JS 設定檔：

1. 確保已將 Hardhat 作為依賴項安裝在 Node.js 專案中，或執行以下命令來執行此操作：

```
npm install --save-dev hardhat
```

2. 導覽至您的 GetBlock 帳戶並安裝 ```getblock.config.js``` 檔案。 複製並貼上到您的工作目錄中；
3. 從專案目錄開啟 ```hardhat.config.js``` 檔案並匯入 getblock 模組：

```javascript
const { getblock } = require('./getblock.config.js');
```

4. 若要將 GetBlock 設定為提供程序，請使用如下所示的憑證修改 Hardhat 設定檔。 使用 *go()* 方法存取整個端點或 *token()* 僅取得令牌。

```javascript
const { getblock } = require('./getblock.config.js'); 

module.exports = {
  defaultNetwork: "sepolia",
  networks: {
    hardhat: {
    },
    sepolia: {
      url: getblock.shared.eth.sepolia.rpc[0].go() // https://go.getblock.io/<ACCESS-TOKEN>/
    },
    goerli: {
      url: `https://go.getblock.io/${getblock.shared.eth.goerli.rpc[0].token()}/` // <ACCESS-TOKEN>
    },
  },
  solidity: {
    version: "0.8.19",
    settings: {
      optimizer: {
        enabled: true,
        runs: 200
      }
    }
  },
  paths: {
    sources: "./contracts",
    tests: "./test",
    cache: "./cache",
    artifacts: "./artifacts"
  },
  mocha: {
    timeout: 40000
  }
}
```
