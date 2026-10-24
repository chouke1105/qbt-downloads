# QBT BT / BLE Verify Tool — Downloads

Public binary downloads and user documentation only. Application source code
and its development history are not hosted in this repository.

## 下載 / Downloads

[最新版下載 / Latest release](https://github.com/chouke1105/qbt-downloads/releases/latest)

| 檔案 | 用途 |
| --- | --- |
| QBT_Setup_Dev_1.3.38_Clean_PC.zip | 建議新電腦使用：安裝程式、ADB、板端部署腳本及README |
| QBT_Setup_Dev_1.3.38.exe | 已有ADB環境時，可單獨安裝Windows工具 |
| QBT_BT_BLE_Menu_CLI_1.5.11_ARM64_20261024.zip | Linux ARM64板端互動選單、部署／啟動／拉取及清理log腳本 |
| SHA256SUMS.txt | 下載檔案SHA-256校驗值 |

## Windows快速開始

1. 下載並完整解壓縮Clean_PC.zip。
2. 執行Install_QBT_Dev.cmd，按提示核准Windows UAC與開發憑證安裝。
3. 連接支援的板子，確認USB/ADB驅動正常。
4. 執行Deploy_Board_Agent.cmd，或在WebUI執行Deploy & verify Board Agent。
5. 開啟QBT，選擇板子與模組，再執行所需測試。

不需安裝Go、Visual Studio、Python或Node.js。Windows藍牙介面、驅動及板端
BlueZ/PipeWire工具仍須支援測項。音訊驗證避免RDP音訊重新導向及其他播放干擾。

## CLI快速開始

完整解壓縮CLI.zip，依README_zh-TW.md或README_EN.md使用01_deploy.cmd，
再選擇02_start_language_menu.cmd、03_start_english.cmd或04_start_chinese.cmd。
06_cleanup_logs.cmd會先預覽，需明確確認才刪除板端舊log。

## 版本與限制

Setup/WebUI1.3.38、Bluetooth Host1.0.24.0、GATT Server1.0.2.0、
Board Agent1.6.18、Menu CLI1.5.11。

這是使用開發自簽憑證的版本，並非公司正式簽章或Microsoft Store版本。
請只在信任發布者及來源後安裝。公開下載不表示所有模組與所有Windows電腦
均已實機認證；experimental模組設定仍須個別驗證。

2026-10-24使用者回報一次Full Validation及三次Board Source→Windows Sink均OK；
不等同全新電腦或長期穩定性驗收。

ADB隨附第三方授權NOTICE；各第三方元件保留原有權利。
本儲存庫不因公開下載而授予應用程式原始碼或商標的額外權利。

## 聯絡 / Contact

Hanson.Chou (Taiwan) — hanson.chou@pactw.com

有問題可聯繫上述信箱。回報請附工具版本、測項及Run ID；分享log前請先
移除個人／機密資訊，勿在公開討論區上傳未遮蔽的裝置資訊或音訊。
