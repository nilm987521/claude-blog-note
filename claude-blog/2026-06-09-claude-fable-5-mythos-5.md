---
title: "Claude Fable 5 與 Claude Mythos 5 正式發布"
tags:
  - Claude Fable 5
  - Claude Mythos 5
  - 新模型
  - 重大公告
  - AI安全
  - Project Glasswing
  - 定價
createdAt: 2026-06-09
lastModified: 2026-06-10
---

# Claude Fable 5 與 Claude Mythos 5 正式發布

**文章網址：** https://www.anthropic.com/news/claude-fable-5-mythos-5

**發布日期：** 2026 年 6 月 9 日

**來源：** Anthropic 新聞

---

## 重點摘要

1. **首個公開的 Mythos 級別模型**：Anthropic 推出 Claude Fable 5，這是首個向大眾廣泛開放的 Mythos 級別模型，在幾乎所有已測試基準中達到最先進水準，涵蓋軟體工程、知識工作、視覺理解、科學研究等領域。Stripe 在早期測試中報告，Fable 5 在一天內完成了原本需要整個工程團隊超過兩個月才能完成的大型程式碼庫遷移。

2. **雙軌發布策略**：同時推出兩個版本 — Claude Fable 5（具備安全過濾器的廣泛可用版）與 Claude Mythos 5（透過 Project Glasswing 計畫，僅向特定網路防禦者和關鍵基礎設施提供商提供的限制存取版）。兩者底層模型相同，差異在於 Mythos 5 在部分領域解除了安全限制。

3. **創新安全機制**：Fable 5 內建安全分類器，針對網路安全、生物學、化學、模型蒸餾等高風險領域的查詢，會自動轉由 Claude Opus 4.8 處理。此機制平均觸發率低於所有對話的 5%，且被拒絕的請求回傳 HTTP 200（`stop_reason: "refusal"`）且不計費。

4. **定價大幅降低**：Fable 5 和 Mythos 5 定價為每百萬輸入 token $10、每百萬輸出 token $50，不到 Claude Mythos Preview 原價的一半。規格方面，預設支援 1M token 上下文視窗，每次請求最多支援 128k 輸出 token。

5. **廣泛平台整合與優惠期**：可透過 Claude API（模型 ID：`claude-fable-5`）、Claude Platform、Claude Code，以及 AWS Bedrock、Google Vertex AI 和 Microsoft Foundry 存取。2026 年 6 月 10 日至 22 日期間，Pro、Max、Team 及企業版座位制用戶可免費使用；6 月 23 日起需消耗用量點數（API 及消費型企業方案則立即完全開放）。

---

## 重要公告

- **新模型上線（Claude Fable 5 & Mythos 5）**：這是 Anthropic 迄今對公眾開放的最強大模型，能夠進行長時間、高度自主的工作，包括數天的大型工程任務。
- **定價策略調整**：相較於上一代 Mythos Preview，新模型定價大幅下調超過 50%，使 Mythos 級別能力首次對廣大開發者和企業具備商業可行性。
- **Project Glasswing 擴展**：與美國政府合作，為合格的網路防禦者及關鍵基礎設施提供商提供 Claude Mythos 5 的有限存取，以支援高風險資安防禦任務。
- **跨雲端平台全面整合**：在 AWS Bedrock、Google Vertex AI、Microsoft Foundry 和 GitHub Copilot 上同步上線，是 Anthropic 模型覆蓋最廣的一次發布。
