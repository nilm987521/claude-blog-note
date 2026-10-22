---
title: "Claude Security now scans continuously and tracks fixes"
tags: ["Claude Security", "資安", "企業功能", "公開測試版", "新功能"]
createdAt: "2026-10-21"
lastModified: "2026-10-21"
---

## 文章資訊

- **來源**: https://claude.com/resources/articles/claude-security-now-scans-continuously-and-tracks-fixes
- **發布日期**: 2026-10-21
- **類別**: 產品公告

## 重點摘要

1. **從一次性掃描升級為持續監控**：Claude Security 從單次掃描進化為持續監控，透過 Claude GitHub App（含 GitHub Enterprise Server）或 GitLab 存取憑證連接代碼庫，建立基線掃描後，隨著程式碼變更自動依風險與複雜度重新掃描。

2. **自動追蹤修復狀態**：Claude 持續核對已知問題與程式碼變更，無論修復是在 Claude Code 還是其他工具中完成，系統都會自動標記已修復；若問題復現，發現項目也會自動重新開啟。

3. **專案知識庫與威脅模型**：每個專案可建立包含部署細節、安全政策等背景資訊的知識庫；系統還能從程式碼自動生成可編輯的威脅模型，引導後續掃描並減少誤報。

4. **API、Webhook 與 MCP 整合**：提供 API 用於列出、讀取、解決或重開發現項目；支援 Webhook 通知外部系統；同時可作為 MCP 連接器在 claude.ai 與 Claude Code 中使用。

5. **採用規模與免費額度**：自今年四月進入公開測試版以來，已有數千個組織使用，累計找出逾百萬個漏洞；企業客戶每月可獲得 25,000 美元免費使用額度，有效期至 2026 年 12 月 31 日。

## 重要公告

- **公開測試版正式開放**：Claude Enterprise 客戶可由管理員在管理控制台啟用
- **底層模型**：由 Anthropic 完整模型家族（包含 Claude Mythos）提供支援，無需 Cyber Verification Program 授權
- **定價優惠**：測試期間每月提供 25,000 美元免費使用額度（至 2026/12/31）
- **角色型存取控制**：管理員可控制各成員的查看、分類與建立專案權限
