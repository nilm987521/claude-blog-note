---
title: "Working at the frontier: How Rakuten builds agents overnight with Claude Fable 5"
tags:
  - Fable5
  - 企業案例
  - Rakuten
  - 自主AI
  - 代理
  - 軟體工程
createdAt: "2026-07-20"
lastModified: "2026-07-20"
---

## 文章資訊

**網址：** https://claude.com/blog/working-at-the-frontier-how-rakuten-builds-agents-overnight-with-claude-fable-5  
**發布日期：** 2026-07-20

## 重點摘要

1. **樂天（Rakuten）推動全公司「AI 化」戰略**：樂天是一家橫跨電商、旅遊、金融科技、數位內容與通訊的全球科技企業，旗下超過 70 個業務。公司推動「AI 化（AI-nization）」戰略，從原本使用 Claude Code 加速軟體開發，進一步擴展至在產品、銷售、行銷、財務等每個業務部門構建 AI 代理。

2. **夜間自主運行的 AI 代理**：工程師可同時啟動多個代理並行作業，例如一個負責市場調研、另一個分析數據，同時審核前晚長時間運行代理產出的成果，協調匯整為最終報告，大幅提升工作效率。

3. **生產程式碼的自主審查流程**：樂天技術團隊將代理部署至數十個最具挑戰性的生產環境程式碼 Pull Request，系統獨立處理每個提交，自動執行測試並驗證結果，再將完成的程式碼呈交工程師進行最終結構審查。

4. **持久計算、記憶與儲存是跨越瓶頸的關鍵**：樂天 Yusuke Kaji 指出：「站在前沿往往意味著解決前所未有的問題。我們早就有強烈直覺：代理需要持久的計算能力、記憶與儲存，才能真正超越對話式 AI 的局限。」

5. **「Working at the frontier」企業案例系列持續擴充**：此文章為 Anthropic 展示 Fable 5 前沿應用的系列案例之一，同系列已涵蓋 Thomson Reuters、Hebbia、Cursor、Cognition 和 Base44 等企業，全面呈現 Fable 5 在不同產業的突破性應用。

## 重要公告

- 樂天正式成為 Claude Fable 5 代理工作流程的旗艦企業案例，展示 AI 代理在大規模電商與企業環境中的實際落地部署。
- 文章呈現了從「使用 AI 工具」到「構建 AI 代理員工」的典範轉移：代理可整夜持續自主工作，讓人類工程師隔天早上直接審核完成的成果。
