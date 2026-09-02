---
title: "Introducing Claude Fable 5.1 and Claude Mythos 5.1"
tags: ["new-model", "claude-fable", "claude-mythos", "performance", "pricing", "watermark", "eu-ai-act"]
createdAt: "2026-09-01"
lastModified: "2026-09-02"
---

# Introducing Claude Fable 5.1 and Claude Mythos 5.1

**文章網址：** https://www.anthropic.com/claude-fable-and-mythos-5-1

## 重點摘要

1. **新模型發布**：Claude Fable 5.1 和 Mythos 5.1 於 2026 年 9 月 1 日正式發布，為 Fable 5 系列的升級版本，也是 Anthropic 首批在文字輸出中內建不可見浮水印的 Claude 模型，符合歐盟 AI 法規的透明度要求。

2. **效能大幅提升**：Fable 5.1 在 Terminal-Bench-Science 0.1（科研任務基準測試）達到 52.6%，相比 Fable 5 的 24.7% 大幅進步超過一倍；在 Terminal-Bench 4.0（編程測試）達到 55.8%（Fable 5 為 42.0%）；Mythos 5.1 在同測試中更達到 60.9%。

3. **定價與成本優化**：定價維持每百萬 input tokens $10、每百萬 output tokens $50，但快取讀取費用大幅降低 75%。模型在低或中等努力程度設定下，可達到與 Fable 5 相似或更佳的效果，但成本顯著降低。

4. **新功能與規格**：支持 100 萬 tokens 上下文長度，單次最多輸出 128,000 tokens。新增兩項測試版功能：對話中途調整努力程度（mid-conversation effort adjustment，可在不重啟對話的情況下調整模型的計算投入），以及內容溯源追蹤（content provenance tracking，協助下游系統驗證生成內容的來源）。

5. **可用性與浮水印**：Fable 5.1 已在 Claude API、Amazon Web Services、Google Cloud 及 Microsoft Azure 等全平台上線；Mythos 5.1 目前僅限美國公司和個人中的受信任訪問計畫（Project Glasswing）參與者。浮水印偵測 API 同步以私人預覽形式向符合歐盟法律資格的機構開放，包括監管機構、執法機構、媒體、事實查核機構及學術研究機構。

## 重要公告

- **新模型上線**：Claude Fable 5.1（`claude-fable-5-1`）現已可在 Claude API 及主要雲平台使用；Claude Mythos 5.1 限受信任訪問計畫參與者。
- **文字浮水印啟用**：這是首批實際攜帶不可見文字浮水印的 Claude 模型，浮水印使用 Google DeepMind SynthID-Text 方法，在生成過程中微調隨機性來源，對內容品質、創意和可讀性無影響，且不含任何用戶個人資訊。
- **浮水印偵測 API 私人預覽**：Anthropic 同步發布浮水印偵測 API（private preview），向合資格機構提供以驗證 Claude 生成的文字。
- **快取費用大降**：快取讀取成本降低 75%，對大量使用 prompt caching 的企業用戶影響顯著。
