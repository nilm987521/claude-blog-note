---
title: "Claude 企業功能更新：集中管理 MCP 連接器授權，支援 Okta 身份提供者"
tags: [企業功能, MCP, 授權管理, Okta, 安全性, 身份提供者]
createdAt: 2026-06-18
lastModified: 2026-06-18
---

## 文章網址

https://claude.com/blog/enterprise-managed-auth

## 重點摘要

1. **管理員可集中佈建 MCP 連接器授權**：企業 IT 管理員現在可透過身份提供者（IdP）為整個組織統一設定 MCP 連接器存取權限，以 Okta 為首批支援的 IdP。用戶首次登入時便可自動獲得對應連接器存取，無需逐一手動授權。
2. **零接觸式使用者體驗**：管理員只需授權一次，使用者即透過既有的 Okta 群組與角色繼承存取權，首次開啟 Claude 時連接器便已就緒，徹底消除終端用戶的手動設定步驟。
3. **精細的存取範圍控制與集中撤銷**：管理員可依 Okta 群組或角色劃定存取範圍，當用戶或部署的 Agent 離職或需要撤銷存取時，直接透過 Okta 統一管理，無需逐個應用程式操作。
4. **多款主流工具支援企業管理授權**：Asana、Atlassian、Canva、Figma、Granola、Linear 和 Supabase 於首批即支援此功能，Slack 即將跟進；基礎協議採用開放標準 XAA（現為 MCP 官方授權擴充規範「Enterprise Managed Auth」）。
5. **更多 IdP 支援即將推出**：Okta 為首批支援的身份提供者，Anthropic 計劃陸續加入對更多身份提供者的支援。

## 重要公告

- **企業安全與管控能力大幅提升**：此次更新解決了企業大規模導入 AI 工具時的核心痛點——集中式存取控制。管理員不再需要依賴每位使用者自行授權，而是透過已有的 IdP 基礎設施統一管理 Claude 的工具存取。
- **基於開放 MCP 標準**：Enterprise Managed Auth 是 MCP 生態系的官方授權擴充規範，由 Anthropic、Microsoft、Okta 及多家 MCP 伺服器廠商共同採納，代表 AI Agent 存取管理進入標準化階段，具有重要的生態系意義。
