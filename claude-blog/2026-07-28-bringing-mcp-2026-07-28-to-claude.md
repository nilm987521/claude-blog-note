---
title: "MCP 2026-07-28 spec: stateless core, coming to Claude"
tags:
  - mcp
  - protocol
  - stateless
  - authorization
  - enterprise
createdAt: 2026-07-28
lastModified: 2026-07-28
---

## 文章資訊

**網址：** https://claude.com/blog/bringing-mcp-2026-07-28-to-claude

## 重點摘要

1. **MCP 移至無狀態核心架構**：本次最重大的規格更新將 MCP 從雙向有狀態協議改為請求/回應模型，伺服器現在可以部署在無伺服器和邊緣基礎設施上，也能透過任何負載平衡器進行水平擴展。

2. **官方擴展框架首次亮相**：MCP Apps（沙盒 iframe 中的伺服器渲染 UI）和 Tasks（長時間執行的非同步操作）作為官方擴展正式推出，讓開發者有正式路徑擴充協議功能，而不需修改核心規格。

3. **企業授權強化**：Authorization 現在與生產環境的 OAuth 2.0 和 OIDC 對齊，可直接整合 Okta、Entra ID 等企業身份系統，無需任何變通方案。

4. **MCP 隧道（研究預覽）**：可讓 Claude 連接私有網路內部的 MCP 伺服器，無需公開 IP、不需開防火牆規則，也不用設定 IP 允許清單。

5. **MCP 月度 SDK 下載量突破 4 億次**：與年初相比成長 4 倍，已成為連接 AI 代理與應用程式的業界標準。

## 重要公告

- **新協議規格**：MCP 2026-07-28 為第五個重大規格版本，正式上線並開始在 Claude、Claude Code、Cowork 等產品中推出支援。
- **無狀態架構**：移除了 initialize 握手和 Mcp-Session-Id 標頭，任何請求都可以落到任意伺服器實例，大幅簡化伺服器部署與擴展。
- **Okta 為首批採用者**：Enterprise-Managed Authorization 擴展已達到穩定狀態，Okta 為首批身份提供商合作夥伴。
