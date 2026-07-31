---
title: "How Datadog built a 'universal machine tool' for Claude Code"
tags:
  - claude-code
  - datadog
  - MCP
  - observability
  - 企業案例
  - 工程師效率
createdAt: "2026-07-21"
lastModified: "2026-07-21"
---

## 文章資訊

- **來源**：[How Datadog built a 'universal machine tool' for Claude Code](https://claude.com/blog/how-datadog-built-a-universal-machine-tool-for-claude-code)
- **發布日期**：2026-07-21
- **分類**：Claude Code / 企業案例

## 重點摘要

1. **Datadog 工程師大規模採用 Claude Code**：Datadog 在過去四個月內，90% 的工程師已將 AI 編碼工具用於生產工作，其中 Claude Code 佔了三分之二的使用量，成為全公司主要的 AI 開發工具。

2. **「通用機器工具」的概念**：Datadog 工程團隊打造了一套以 Datadog MCP Server 為核心的「通用機器工具」，將 Datadog 的完整可觀測性能力（日誌、指標、追蹤記錄、儀表板等）以 AI 代理可呼叫的工具形式封裝，讓 Claude Code 能透過自然語言直接存取生產環境數據。

3. **自然語言查詢生產數據**：工程師可直接在 Claude Code 終端機中以自然語言下指令，例如「拉取過去六小時 checkout 服務的所有追蹤記錄，並告訴我發生了什麼變化」，Claude 即可即時撈取並分析相關遙測數據，大幅縮短除錯與事故回應的時間。

4. **官方 Claude 插件上架**：該整合現已以官方插件形式發布，工程師只需在 Claude Code 中執行 `/plugin install datadog@claude-plugins-official`，完成 `/ddsetup` 設定後即可立即使用，整合 Datadog 帳號下的所有可觀測性資源。

5. **跨平台通用架構**：Datadog MCP Server 並不限於 Claude Code，同樣支援 Cursor、ChatGPT 及其他相容 MCP 的 AI 工具，體現了「通用」的設計理念，讓同一套整合可橫跨不同 AI 開發環境使用。

## 重要公告

- Datadog 成為 Claude Code 企業整合的重要標竿案例，展示了可觀測性平台如何透過 MCP 深度融入 AI 輔助開發工作流程。
- 官方 Claude 插件（`datadog@claude-plugins-official`）正式上架，提供自動更新及預設配置，是迄今最完整的 Datadog × Claude Code 整合方案。
