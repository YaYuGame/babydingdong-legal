# babydingdong-legal

《寶貝叮咚》公開網頁：隱私政策／使用條款／帳號刪除申請。

- **唯一全文來源**：本站（GitHub Pages）
- App 以 WebView 開啟本站，不再內嵌條款本文
- 生效日期：2026年8月15日（與預計上架日對齊）
- 本文件為營運草案，不構成法律意見

## 線上網址（GitHub Pages）

部署後：

| 頁面 | URL |
|------|-----|
| 首頁 | https://yayugame.github.io/babydingdong-legal/ |
| 隱私政策 | https://yayugame.github.io/babydingdong-legal/privacy/ |
| 使用條款 | https://yayugame.github.io/babydingdong-legal/terms/ |
| 帳號刪除 | https://yayugame.github.io/babydingdong-legal/delete-account/ |

Play Console：隱私權政策填「隱私政策」URL；Data safety 帳號刪除填「帳號刪除」URL。

## 怎麼更新（從 BabyDingDong 主專案）

條款**原稿**放在主專案的 `babydingdong-legal/`。  
公開站是另一個 repo：`YaYuGame/babydingdong-legal`（GitHub Pages）。

改完後在**主專案根目錄**執行：

```bash
./scripts/publish_legal_web.sh          # 同步並推送
./scripts/publish_legal_web.sh --dry-run # 只預覽差異
```

流程：改 `babydingdong-legal/` →（可選）commit 進 BabyDingDong → 跑腳本推公開站。  
App WebView 會讀線上站，**不必為改條款發 App 版**（除非改了網址）。

## 本機預覽

```bash
python3 -m http.server 8080
```
