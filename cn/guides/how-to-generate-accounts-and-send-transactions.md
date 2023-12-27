---
lastUpdated: October 23, 2023
---

# 如何生成賬戶並發送交易

在本指南中，GetBlock 團隊將闡明我們的用戶如何實際連接到區塊鏈節點。 在區塊鏈中生成帳戶和發送交易是我們首先要介紹的兩個操作。

在區塊鏈中，“賬戶”應該被稱為一對私鑰和公鑰。 區塊鏈通過這些密鑰對“識別”其用戶和余額。

與傳統計算解決方案中的登錄/密碼對不同，在現代區塊鏈中，每個帳戶只能使用私鑰來恢復。

因此，要將交易廣播到去中心化網絡，我們首先需要創建（或恢復）我們的帳戶。

## 創建賬戶

首先，我們需要設置一個屬於每個 GetBlock 用戶的 API 密鑰。 整套交互是通過 Web3.js 庫組織的。 在下面的演示中，我們嘗試在世界領先交易所幣安的可編程區塊鏈【幣安智能鏈】(https://getblock.io/nodes/bsc/)中創建賬戶：

```javascript
const Web3 = require('web3');
const apikey = process.env['apikey'];
const network = 'testnet'; // Change to mainnet for production
const chainId = 97; // 97 is BSC testnet, 95 is BSC mainnet
const node = 'https://go.getblock.io/<ACCESS-TOKEN>/';
const web3 = new Web3(node);
// Generate new address and private key
const accountTo = web3.eth.accounts.create();
console.log(accountTo);
```

這就是我們在 BSC 測試網創建帳戶的方式。 我們可以使用新密鑰對生成一個新帳戶，也可以僅從私鑰恢復帳戶。

```javascript
// Restore account from private key
const privateKey = process.env['privateKey'];
const accountFrom = web3.eth.accounts.privateKeyToAccount(privateKey);
```

您可能會問，當我們與幣安智能鏈交互時，“eth”是什麼意思？ 沒錯，這反映了幣安智能鏈與以太坊虛擬機完全兼容的事實。

## 發送交易

在區塊鏈中，交易應該經過簽名（授權）才能“包含”到區塊鏈中（由礦工或驗證者的共識確認）。

這是我們的交易是如何創建的。 0.01 ETH 用於演示。

```javascript
const createSignedTx = async (rawTx) => {
rawTx.gas = await web3.eth.estimateGas(rawTx);
return await accountFrom.signTransaction(rawTx);
}

const sendSignedTx = async (signedTx) => {
// You can use signedTx.rawTransaction as params for
// calling eth_sendRawTransaction JSON-RPC method
web3.eth.sendSignedTransaction(signedTx.rawTransaction).then(
console.log
);
}

const amountTo = "0.01" // ether
```

這就是交易在被納入區塊鏈之前的樣子。 一旦簽名，就可以發送給礦工。

```javascript
const rawTx = {
to: accountTo.address,
value: web3.utils.toWei(amountTo, 'ether'),
chainId: chainId
};

createSignedTx(rawTx).then(sendSignedTx)
```

就是這樣：您的賬戶一切順利，交易已成功提交！

如果您有興趣運行或分叉此代碼，請不要猶豫再檢查一次：[https://replit.com/@getblock/BSCKeyGenAndSignTx](https://replit.com/@getblock /BSCKeyGenAndSignTx)
