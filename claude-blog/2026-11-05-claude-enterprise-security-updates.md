---
title: "More visibility and control over Claude Enterprise for security teams"
tags: ["企業安全", "Claude Enterprise", "新功能", "Security Center", "Inference Hooks", "beta"]
createdAt: "2026-11-05"
lastModified: "2026-11-05"
---

# More visibility and control over Claude Enterprise for security teams

**文章網址：** https://claude.com/resources/articles/claude-enterprise-security-updates

## 重點摘要

1. **Security Center（Beta）**：新的組織設定頁面，可將 Claude 聊天、Cowork 及 Claude Code 的現有配置與 Anthropic 建議設定進行對比，並可下載報告供稽核使用。

2. **Inference Hooks（正式上線）**：分為 Prompt Hook（檢查提示詞）及 Pre-tool-call Hook（在工具呼叫執行前檢查），可整合企業現有的 DLP 及資安政策工具。

3. **集中管理主控台（Beta）**：於 admin.claude.com 提供跨組織的統一管理介面，支援 SSO、SCIM 目錄同步、網域驗證、群組管理，以及多個身份提供商（IdP）。

4. **存取控制（Beta）**：管理員可透過一個 Admin API 呼叫強制登出特定成員的所有工作階段、自助管理 IP 允許名單、在受管裝置上封鎖個人帳號以防止影子 IT，以及限制使用者可用的工作區資料夾。

5. **EDR 整合（Beta）**：管理員可在 macOS 和 Windows 本地 Cowork 虛擬機器中執行 EDR 感測器，Claude 會驗證感測器簽章，感測器以偵測模式運作（僅回報、不封鎖），此功能暫不支援雲端 Cowork 工作階段。

## 重要公告

- **新功能**：Security Center、集中管理主控台、EDR 整合均以 Beta 形式推出。
- **正式上線**：Inference Hooks 從 Beta 轉為正式可用（GA）。
- **適用對象**：Claude Enterprise 方案用戶；無新增定價或新模型發布。
