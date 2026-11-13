---
title: "Operate Claude Managed Agents inside your security perimeter"
tags: ["managed-agents", "self-hosted", "enterprise", "security", "infrastructure"]
createdAt: "2026-11-12"
lastModified: "2026-11-12"
---

# Operate Claude Managed Agents inside your security perimeter

**文章網址：** https://claude.com/resources/articles/self-hosted-claude-managed-agents

## 重點摘要

1. **自架 Claude Managed Agents 開放私人測試版**：企業現在可以在自己的雲端或本地環境中運行完整的 Managed Agents 服務，不再依賴 Anthropic 的託管基礎設施。

2. **架構設計**：Agent 的執行環境（harness）、沙盒、憑證管理和對話歷史都在自己的環境中運行。模型請求路徑可自選，支援直接呼叫 Anthropic 或透過 Amazon Bedrock、Google Agent Platform、Microsoft Foundry 等雲端服務商。

3. **四大安全原則**：
   - 大腦與執行分離（harness 呼叫 Claude，沙盒執行工具程式碼）
   - 憑證不進入沙盒（透過沙盒外代理注入）
   - 網路存取限制（可設定白名單）
   - 完整稽核追蹤（可透過 OpenTelemetry 匯出至既有監控工具）

4. **資料合規**：對話歷史儲存於自有資料庫；已啟用零資料保留（ZDR）的組織，其 Claude 請求同樣適用相同條款。

5. **開發體驗一致**：開發者使用與託管版本相同的核心 API，無需更換程式碼。

## 重要公告

- **新功能**：自架 Claude Managed Agents 現已開放私人測試版，請透過 Anthropic 客戶代表申請存取。
