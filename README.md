# Real-Time Color Sync (跨裝置同步換色螢幕)

可以直接點右邊連結:[[連結](https://firebase.google.com/)](https://chang0107.github.io/BlackWrite/)

這是一個簡單但強大的網頁工具，能夠在 **手機、平板、電腦** 等多平台瀏覽器上即時同步螢幕顏色。只需點擊螢幕任何處，所有開啟此網頁的裝置都會同步切換 **全黑** 或 **全白** 畫面。

## 🌟 功能特點
* **跨平台支援**：支援 Windows, macOS, Android, iOS 等所有主流瀏覽器。
* **毫秒級同步**：利用 Firebase Realtime Database 達成極低延遲的即時反應。
* **狀態持久化**：即使重新整理網頁，畫面也會維持在最後一次切換的顏色。
* **簡約設計**：無 UI 干擾，全螢幕純色體驗。

## 🛠 使用技術
* **Frontend**: HTML5, CSS3, JavaScript (ES6+)
* **Backend as a Service**: [Firebase Realtime Database](https://firebase.google.com/)
* **Hosting**: GitHub Pages

## 🚀 快速上手

### 1. 複製專案
將此儲存庫複製到你的電腦，或直接在 GitHub 上建立新檔案。

### 2. 設定 Firebase
由於此專案需要資料庫來達成同步，你需要：
1. 前往 [Firebase Console](https://console.firebase.google.com/)。
2. 建立新專案並新增 **Realtime Database**。
3. 在專案設定中取得你的 `firebaseConfig` 程式碼。
4. 將 `index.html` 中的配置區塊替換為你的金鑰：
   ```javascript
   const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       databaseURL: "YOUR_DATABASE_URL",
       // ... 其他參數
   };
   ```

### 3. 部署
將程式碼推送到 GitHub 後，開啟 **Settings > Pages**，選擇 `main` 分支進行部署。

## 📖 使用情境
* **攝影補光**：多台手機同時變白作為簡易補光燈。
* **信號傳遞**：在安靜場合透過螢幕顏色切換傳遞簡單信號。
* **技術示範**：展示 WebSocket 或即時資料庫同步原理的入門範例。
