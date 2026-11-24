---
title: "The enterprise guide to securing coding agents"
tags: ["security", "enterprise", "coding-agents", "best-practices", "prompt-injection"]
createdAt: "2026-11-23"
lastModified: "2026-11-23"
---

## 文章資訊

**來源：** https://claude.com/resources/articles/enterprise-guide-to-securing-coding-agents

## 重點摘要

- **目標是限制風險，而非完全消除：** 程式碼代理程式已在許多企業中撰寫、審查和合併程式碼，因此重點是讓代理程式風險「可見且可控」（legible and bounded），而非徹底阻止其使用。
- **主要 AI 特定風險：** 包括憑證外洩、代理程式繼承開發者過高權限、未審查的依賴套件與擴充功能（含 MCP 伺服器、插件、技能）、透過已允許服務的資料外洩，以及隱藏在代理程式所讀內容中的提示注入（prompt injection）。
- **分層防禦策略：** 模型對齊與分類器能攔截惡意行為，但並非百分之百可靠。應搭配確定性邊界，如「預設拒絕」的權限規則、hooks、沙箱環境和出站白名單，以限制損害範圍。
- **具體控制措施：** 使用短期有效、無金鑰的憑證，並為 CI 代理程式設立獨立身分。將依賴套件限制在內部 registry、鎖定版本、縮小網路白名單（含 DNS）。對不可逆的高風險操作（如正式環境遷移或 IAM 變更）要求人工核准。
- **集中政策管理與稽核追蹤：** 使用個別開發者無法覆蓋的集中式設定，並保留 session 遙測資料以便事後重建事件經過。建議先在低風險的 repo 試行，再擴展至全面部署。

## 重要公告

- 此為企業資安指南，提供保護程式碼代理程式的具體最佳實踐，無新產品或功能發布
