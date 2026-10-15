---
title: "Agent observability on the Claude Platform"
tags: ["agent", "observability", "opentelemetry", "platform", "tracing"]
createdAt: "2026-10-14"
lastModified: "2026-10-14"
---

## 文章資訊

- **來源網址**: https://claude.com/resources/articles/agent-observability-on-the-claude-platform
- **發布日期**: 2026-10-14

## 重點摘要

1. **OpenTelemetry 追蹤進入公開測試版**：Claude Managed Agents、Messages API 及 Claude SDK 現可將 OTel 追蹤資料傳送至任何相容 OTel 的工具，讓開發者能追蹤每個 agent 執行步驟。

2. **追蹤內容涵蓋範圍廣泛**：每次 agent 回合、模型呼叫與工具使用均會匯出為標準 OTel trace，包含延遲時間、token 用量及識別碼，MCP server 呼叫亦包含在內。

3. **設定方式**：Managed Agents 和 Messages API 需在 Claude Console 中新增追蹤目的地；Claude SDK 則會自動匯出追蹤資料。

4. **廣泛的工具相容性**：遵循 OpenTelemetry GenAI 語意規範，可與 Grafana Cloud、Honeycomb、Sentry、Splunk（一般觀測）及 Arize、Braintrust、Datadog、Langfuse、LangSmith、New Relic、PostHog（評估與品質）等工具整合。另支援 Databricks Unity Gateway 進行全組織 token 用量追蹤。

5. **實際應用案例**：Foxglove、Ramp、Sterling Labs、FloQast 等客戶已利用原生 OTel 匯出功能評估 agent 表現、從生產資料改進系統，並稽核 agent 行為。

## 重要公告

- **新功能**：Claude Platform 正式推出 OpenTelemetry 追蹤支援（公開測試版），為 agent 開發提供原生可觀測性能力。
- 設定文件：platform.claude.com/docs/en/manage-claude/opentelemetry
