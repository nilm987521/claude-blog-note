---
title: "Inference hooks: inline data loss prevention for Claude Enterprise"
tags:
  - enterprise-ai
  - security
  - dlp
  - data-loss-prevention
  - claude-enterprise
createdAt: "2026-08-05"
lastModified: "2026-08-05"
---

## 文章資訊

- **原文網址**：https://claude.com/blog/claude-enterprise-inference-hooks
- **發布日期**：2026-08-05
- **分類**：Enterprise AI

## 重點摘要

1. **即時 DLP 稽核機制**：Inference hooks 讓企業合規團隊能在每次推論請求送達 Claude 之前，先通過組織自有的安全伺服器進行「允許／拒絕」審核，覆蓋範圍包含聊天、Claude Code、Claude Cowork 等所有 Claude Enterprise 介面。

2. **伺服器端稽核，零裝置安裝**：稽核點設置於 Anthropic 伺服器端（請求離開用戶端後、推論開始前），不需在使用者裝置上安裝任何額外軟體，即可統一管控所有服務入口。

3. **整合現有企業 DLP 工具**：可直接對接 Netskope、Palo Alto Networks、Proofpoint、Zscaler 等主流企業安全系統，也支援自行建置的安全伺服器。

4. **彈性部署選項**：提供 shadow mode（僅記錄不攔截）、基於角色的排除設定、以及百分比滾動部署，方便企業分階段導入。

5. **當前限制**：判定結果僅支援「允許」或「拒絕」，無法改寫或遮蔽敏感內容；圖片附件（如文件截圖）無法進行文字內容檢查。

## 重要公告

- **新功能上線**：Inference hooks 現已以 **beta 版**向 Claude Enterprise 客戶開放，是企業在 AI 工作流程中落實資料防洩漏（DLP）政策的重要里程碑。
- **應用場景**：除了 DLP 之外，也支援即時記錄存檔（作為 Compliance API 輪詢的推送替代方案）、提示詞遙測，以及自訂政策引擎（如模型白名單、專案範圍限制）。
