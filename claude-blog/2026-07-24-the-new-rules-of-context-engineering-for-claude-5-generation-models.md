---
title: "The new rules of context engineering for Claude 5 generation models"
tags:
  - context-engineering
  - claude-5
  - best-practices
  - claude-code
  - agents
createdAt: 2026-07-24
lastModified: 2026-07-24
---

## 文章資訊

- **來源**：Claude 部落格
- **網址**：https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models
- **發布日期**：2026-07-24

## 重點摘要

1. **上下文工程的定義**：上下文工程（Context Engineering）是指設計 Claude 所接收的「所有資訊」的實踐——不只是聊天框中輸入的提示詞，還包含系統提示、Skills、CLAUDE.md 文件、記憶及其他來源，這些組合在一起共同構成 Claude 真正接收到的完整上下文。

2. **提示詞只是冰山一角**：當你傳送訊息給 Claude 時，提示詞只是整體上下文的一小部分；大多數上下文是由外部來源自動組裝而成，因此僅僅優化提示詞遠遠不夠。

3. **上下文 vs. 提示詞的關鍵差異**：提示詞針對單一具體請求設計，而上下文則跨多個請求通用使用，因此上下文不能太過具體，需要設計得更具通用性與彈性。

4. **Claude 5 世代的新規則**：隨著 Claude 5 世代模型能力的大幅提升，結構化設計（architecture）的重要性已超越措辭（phrasing）。模型品質夠高，意味著「如何組織信息」比「如何表達信息」影響更大。

5. **對 Claude Code 與代理開發的影響**：在使用 Claude Code 或建立自訂代理時，上下文工程對最終結果有重大影響。開發者應主動設計好 CLAUDE.md、系統提示與 Skills，而非僅依賴臨時提示詞。

## 重要公告

- 本文代表 Anthropic 對 Claude 5 世代最佳使用實踐的官方指引轉向，強調從「提示詞工程」思維升級為「上下文工程」思維
- 對 Claude Code 使用者與代理開發者尤為重要，建議重新檢視整體上下文架構設計
