---
title: "Linked billing on the Claude Platform"
tags: ["billing", "claude-platform", "api", "enterprise", "product-update"]
createdAt: "2026-11-17"
lastModified: "2026-11-17"
---

## 文章資訊

- **原文網址**：https://claude.com/resources/articles/linked-billing-on-claude-platform
- **發布日期**：2026-11-17
- **分類**：Product updates, Claude Platform
- **閱讀時間**：約 4 分鐘

## 重點摘要

1. **連結帳單（Linked Billing）正式進入測試版**：第三方平台（如程式碼代理工具、工作流程自動化工具）的客戶，現在可以讓 Claude API 的使用費直接計入自己的 Claude Platform 帳戶，不需要共享 API 金鑰。

2. **安全性大幅提升**：由於 API 金鑰不再需要在平台與客戶之間傳遞，平台方不必儲存、加密或輪換客戶的金鑰，降低了安全風險。

3. **平台方的好處**：Anthropic 負責主持授權流程與帳務，平台方無需自行建構計量或發票系統。平台方可透過 Console 或使用量與費用分析 API（測試版）查看每位客戶的請求次數、Token 用量與使用的模型，並可自行決定每筆請求由平台還是客戶付費。

4. **客戶端的控制彈性**：客戶可設定每個平台的每月消費上限，在 Console 中查看各平台的費用，並可隨時解除連結。現有的 Anthropic 合約用量或隨用隨付方案皆適用。

5. **限制事項**：請求仍在平台的組織環境下執行，因此客戶組織層級的設定（如 IP 許可清單、加密金鑰、資料保留政策等）並不適用。

## 重要公告

- **新功能**：Linked Billing（連結帳單）正式進入測試版，支援的平台包括 Asana、ClickHouse、Factory、Gumloop、Harness、Higgsfield AI、Kilo Code、Linear、Mintlify、Omni、Railway、Ramp、Tines、Warp 等多個第三方服務。
- 平台方可在 Console 建立應用程式並參考連結帳單文件來接入此功能；客戶則可在 Claude Marketplace 找到支援的平台並進行連結。
