## Windows 安裝 Flutter 指南

### 步驟1: 確保你的電腦符合以下的基本需求：

- **作業系統**：Windows 10 或更新的版本 (64位元), 基於 x86-64。
- **磁碟空間**：至少需要2.5GB的空間（不包含IDE/工具的空間）。

### 步驟2: 下載 Flutter SDK

至[官網](https://docs.flutter.dev/)下載最新版本的 Flutter SDK 安裝包：
- 解壓縮zip檔案，將包含的flutter文件夾放到你希望的安裝位置（例如`D:\dev\flutter`）。

⚠️ 注意：
- 安裝路徑不要包含特殊字元或空格與中文。
- 不要安裝到需要管理員權限的目錄，如 `C:\Program Files\`。

### 步驟3: 更新你的環境變數

1. 從「開始搜索欄」輸入「env」，選擇「編輯你帳戶的環境變數」。
 
   ![編輯環境變數](https://github.com/EduCatCode/Learn_Flutter/assets/148319229/7e668a1d-8159-4cc4-998f-04b3548c21a9)
   
2. 在「使用者變數」區域，找到並選擇名為 `Path` 的項目，然後進行如下操作：
   - 點選「新增」並輸入 `flutter\bin` 的完整路徑。

   | Path | 新增 |
   | :---: | :---: |
   | ![Path 變數](https://github.com/EduCatCode/Learn_Flutter/assets/148319229/42f068a5-eff7-432c-8268-547912152fb9) | ![新增 Path](https://github.com/EduCatCode/Learn_Flutter/assets/148319229/0283caf7-c0cb-4275-8898-2bdbab065d3a) |


🔍 提示：要讓這些變更生效，你需要關閉並重新開啟任何現有的命令視窗。

### 步驟4: 執行 `flutter doctor` 命令

在你已經更新了 PATH 環境變數之後，你需要驗證你的開發環境是否已正確設定。為此，你可以使用 Flutter 提供的 `flutter doctor` 命令，它會檢查你的機器上是否設置了所需的依賴項，並輸出任何推薦的解決方案。

請依照以下步驟操作：

1. 打開命令提示字元：
   - 按下 `Windows` 鍵，開啟「開始」選單。
   - 在搜索欄輸入 `cmd` 或「命令提示字元」。
   - 從搜索結果中選擇「命令提示字元」並打開它。

2. 在命令提示字元中，輸入以下命令並按下 `Enter` 鍵：

```shell
flutter doctor
