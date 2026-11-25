---
title: "MCP servers can now ship skills, run tasks, and more with Claude"
tags: ["mcp", "skills", "tasks", "elicitation", "developer", "enterprise"]
createdAt: 2026-11-24
lastModified: 2026-11-25
---

# MCP servers can now ship skills, run tasks, and more with Claude

**文章網址：** https://claude.com/resources/articles/skills-over-mcp-tasks-and-more

## 重點摘要

1. **Skills over MCP（公開測試版）：** MCP 伺服器現在可隨工具發布「技能（Skills）」，提供多步驟工作指引與最佳實踐；技能僅在需要時載入，大幅降低 context 佔用。已有 Shopify、HubSpot、Atlassian、Carta 等合作夥伴接入，預設支援 Pro、Max、Ultra 方案，Team 方案需管理員啟用，Enterprise 支援即將推出。

2. **Tasks 正式上線（GA）：** 伺服器可在背景執行耗時操作或完整 Agent 迴圈，Claude 無需等待即可繼續工作，完成後再取回結果。ZoomInfo 利用此功能進行更深入的帳戶與聯絡人研究。

3. **Elicitation 正式上線（GA）：** 伺服器可在操作途中暫停並透過表單或連結向使用者請求確認，適用於需要授權的操作（如消費、刪除資料）。Supabase、Railway、GitHub 等已採用此機制。

4. **File Uploads 即將推出：** Claude 將能直接傳送 PDF、試算表、圖片等檔案至 MCP 伺服器，無需透過 context 視窗中繼，計畫適用於 Pro、Max、Ultra 及符合條件的 Team/Enterprise 方案。

5. **整體 MCP 效能大幅提升：** 透過「工具搜尋」機制在多伺服器環境中減少超過 85% 的 context 佔用；新版規格改為無狀態設計，更易於建構與維護；Enterprise Managed Auth 擴充套件讓管理員一次授權後使用者自動連線；MCP Apps 擴充套件可在對話旁或全螢幕顯示完整介面。

## 重要公告

- **MCP 推出兩周年：** MCP 自兩年前作為開放標準推出，現已由 Agentic AI Foundation 託管，每月 SDK 下載量超過 **7 億次**，Claude 現有超過 **10,000 個 MCP 連接器**。
- **四大新功能同步發布：** Skills（Beta）、Tasks（GA）、Elicitation（GA）、File Uploads（即將推出），全面強化 MCP 生態系能力。
- **開放標準：** 所有功能均基於開放 MCP 規格及其擴充套件，相容的用戶端均可支援，不限於 Claude。
