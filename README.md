# Chatbot

Prediction Market 平台 Chatbot 的規劃文件。主排期（`prediction-docs/roadmap/schedule.md`）把 Chatbot 列為延後項目，本資料夾補上規格與排期**提案**，尚未排入主排期。

| 文件 | 內容 |
| --- | --- |
| [`mvp.md`](./mvp.md) | 最小可行方案：範圍與定案、功能模組、選單規則、資料表、成功標準、取捨、範圍收斂紀錄 |
| [`roadmap.md`](./roadmap.md) | 未來可擴充方向：功能清單（解決什麼、前置依賴、合規注意）、階段順序、MVP 已預留的擴充點 |
| [`schedule.md`](./schedule.md) | 實作排期：stage 定義、各 sprint 工作與工時、驗收點、待拍板事項、風險（格式比照 `prediction-docs/roadmap/schedule.md`） |

## 結論一覽

- **形態**：前端是插件式 Widget，後端是平台的共用功能模組
- **第一版範圍**：按鈕式決策樹問答＋非同步工單＋管理後台；入口為 forum、voting
- **使用者**：未登入可使用；開工單需登入，客服回覆顯示在 chatbot 聊天室內
- **合規**：Chatbot 不得對議題結果提供任何預測、判斷或建議
- **排期**：4 個 sprint、8 週；人力與啟動時間為假設，待拍板

## 與既有設計文件的關係

- `prediction-docs/design/prediction-system-design.md` §3.3.5 原把 Chatbot 定位為「推薦文章與議題、彙整討論與投票狀態」的純讀取端；本版改做客服導覽，推薦與彙整列為未來擴充
- 同文件 §3.3.4.1 規定**客服工單是 CRM 的單一來源**；第一版先自建工單表、欄位對齊 CRM，CRM 上線後併入
