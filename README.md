# 你吃出了什麼人生？— 營養人生模擬器

一款手機優先的營養學期末互動網頁遊戲。從 20 歲到 60 歲，透過 10 次飲食選擇，得到不同的故事結局與營養回饋。

## 開始遊玩

直接開啟 `index.html`，不需要安裝任何套件或執行伺服器。

## 放到 GitHub Pages

1. 在 GitHub 建立一個新 repository，例如 `nutrition-life-game`。
2. 上傳 `index.html`（和這份 `README.md`）到 repository 根目錄，並 commit。
3. 進入 repository 的 **Settings → Pages**。
4. 在 **Build and deployment** 將 Source 設成 **Deploy from a branch**；Branch 選 **main**，資料夾選 **/(root)**，按 **Save**。
5. 部署完成後，GitHub Pages 會顯示可公開遊玩的網址，格式通常是 `https://你的帳號.github.io/nutrition-life-game/`。

## 自訂內容

- **修改 10 個關卡**：編輯 `index.html` 中的 `EVENTS` 陣列。
- **更換選項與文字回饋**：修改每個事件的 `options` 與 `reply`。
- **修改數值**：每個選項的 `delta` 依序為 `[能量管理, 營養均衡, 健康習慣]`。
- **修改結局**：編輯 `getEnding()`。
- **修改畫面風格**：調整 `<style>` 中的 CSS。

## 目前版本的設計說明

- 10 個關鍵事件；每個事件 3 個選項。
- 每次選擇後有簡短的營養學提示。
- 三個遊戲化數值以及四個可能結局。
- 有簡單的前次選擇敘事回應與結果複製功能。
- 免登入、無資料庫、無外部套件或第三方圖片資源。
- 遊玩時間以一般閱讀速度估計約 4–5 分鐘，**沒有強制倒數計時**。

> 注意：數值和結局是教育性遊戲機制，並非經驗證的健康評估模型，也不代表醫療診斷或個人未來預測。正式作業發表前建議依教材及可信的營養指南核對文本。
