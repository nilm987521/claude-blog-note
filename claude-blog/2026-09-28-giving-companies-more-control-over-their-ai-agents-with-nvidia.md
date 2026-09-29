---
title: "Giving companies more control over their AI agents, with NVIDIA"
tags: ["代理程式", "安全", "NVIDIA", "企業", "Claude Managed Agents"]
createdAt: "2026-09-28"
lastModified: "2026-09-28"
---

## 文章資訊

- **來源：** https://claude.com/blog/giving-companies-more-control-over-their-ai-agents-with-nvidia
- **發布日期：** 2026-09-28
- **分類：** 代理程式（Agents）

## 重點摘要

1. **Anthropic 與 NVIDIA 策略合作**：雙方共同推出「開放代理程式安全平台」（Open Agent Safety Platform），透過多層防護架構，讓企業在部署 AI 代理程式時擁有更高的安全性與控制力。

2. **Claude Managed Agents 正式推出**：這套可組合的 API 套件專為在生產環境中建構及部署代理程式而設計。其核心特色是透過憑證保險庫（Credential Vault）集中管理代理程式所需的帳密，讓代理程式本身永遠無法直接接觸憑證，大幅降低洩露風險。

3. **三層獨立防護架構**：
   - **模型層**：Claude 內建的安全防護機制
   - **Managed Agents 層**：憑證隔離與完整稽核追蹤
   - **NVIDIA OpenShell 層**：以數學策略驗證精確控制代理程式的存取權限與執行範圍

4. **完整的企業級功能**：平台涵蓋安全沙盒、長時間自主執行（支援中斷後恢復）、多代理程式協作編排，以及具備範圍限制的權限治理與執行追蹤功能。

5. **主要企業已率先採用**：Notion、Rakuten、Asana 等公司已跨部門（工程、財務等）部署代理程式，處理複雜任務的同時維持嚴格的安全管控。

## 重要公告

- **新功能發布**：Claude Managed Agents 即日起正式推出，可立即使用。
- **開源工具**：NVIDIA OpenShell 以 Apache 2.0 授權開源，已發布於 GitHub，提供可數學驗證的代理程式權限政策。
- **安全哲學轉變**：強調「不仰賴單一防護層」的縱深防禦設計，確保整體系統在任一層失效時仍保有保護能力。
