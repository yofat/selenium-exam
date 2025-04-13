# Selenium IDE
## 網址：https://www.selenium.dev/selenium-ide/
---
# 最初
### 你需要去安裝與你的瀏覽器相對應的 IDE 版本
### 然後他會出現在你的瀏覽器插件那邊
### 在這個圖案
![image](https://github.com/user-attachments/assets/39d35ede-f320-4a5b-a7b4-3a4879f2a5b9)
## 測試
### 按下左側邊欄menu頂部（測試標題右側）的 「+」符號，命名並 click 「Add」，即可添加新測試。
### 添加後，您可以手動輸入命令，或點擊 IDE 右上方的「錄制」圖案。
## 分組
### 測試可以組合成Suites。
### 創建專案時，會建立一個默認Suite，並自動將第一個測試添加到該套件中。
### 要創建和管理套件，請進入測試套件面板。單擊左側邊欄menu頂部的下拉選單並選擇「Test Suites」，即可進入面板。
## 儲存
### 按下 3.5 磁碟片的圖案就可以存檔
---
# 程式運行
## 網址：https://www.selenium.dev/selenium-ide/docs/en/introduction/command-line-runner
### 儲存下來之後可以將它存成程式嗎，並且在本機端運行
### 而要能夠運行就需要使用 npm ，npm 要下載 node.js 才可以使用
## 安裝
### 網址：https://nodejs.org/en/download/current
### 照著裡面的文字輸入進 powershell 就好了
```powershell
# Download and install fnm:
winget install Schniz.fnm
# Download and install Node.js:
fnm install 23
# Verify the Node.js version:
node -v # Should print "v23.11.0".
# Verify npm version:
npm -v # Should print "10.9.2".
```
## 環境
### 接著還要設定環境變數
### 在放大鏡中或是直接按一下開始，並且輸入還進變數
### 右下角有一個環境變數的按鈕
### 接著在系統變數中找 PATH 對他點一下，然後按下面的編輯
### 將 npm 的路徑加進去
```txt
C:\Users\user\AppData\Roaming\npm
```
### 這時候才可以在 powershell 中使用
### 接著再回去剛剛的網站複製以下指令，並貼到 powershell 中去執行
```powershell
npm install -g selenium-side-runner
```
### 以及安裝瀏覽器的 driver
```powershell
npm install -g chromedriver
```
### 然後把 chromedriver 的路徑加到環境變數
```txt
C:\Users\user\AppData\Roaming\npm\node_modules\chromedriver\lib\chromedriver
```
## 執行
### 最後輸入這個指令就可以執行
```powershell
selenium-side-runner 檔案位置
```
