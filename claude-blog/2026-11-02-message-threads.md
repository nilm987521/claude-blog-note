---
title: "Make long-running agents faster with message threads"
tags: ["API", "Messages API", "效能", "代理人", "公測"]
createdAt: 2026-11-02
lastModified: 2026-11-03
---

## 文章資訊

- **來源**：Claude 部落格
- **網址**：https://claude.com/resources/articles/message-threads
- **發布日期**：2026-11-02
- **類別**：公告 / Claude 平台

## 重點摘要

1. **Message Threads 進入公測**：Messages API 新增 `thread` 參數，允許代理人在長時間對話中只傳送新訊息，而非每次都重送完整對話歷史，藉此降低延遲。

2. **降低首字延遲（TTFT）**：在長時間工作階段（如編程代理人進行數百次請求時），重送完整歷史會拖慢首字回應速度。Message Threads 可有效減少這段等待時間。

3. **運作方式**：第一次請求傳送完整對話並建立 thread；後續請求只需附上前一次回應的 ID 與新訊息即可，大幅縮小每次的請求大小。

4. **儲存與到期**：Thread 內容保存在記憶體中並加密，不寫入磁碟；最後一次請求後 5 分鐘到期。Token 用量不變，Claude 仍讀取完整對話內容。

5. **實測成效**：對大多數 Claude Code 使用者預設啟用後，500k 至 100 萬 token 的請求中，中位數首字延遲降低約 35%。

## 重要公告

- **新功能**：Message Threads（訊息串）正式進入**公測階段**。
- **適用平台**：原生 Claude 平台、AWS 上的 Claude Platform、Microsoft Foundry 中的 Claude，以及 Google Cloud 上的 Anthropic 託管 Claude 模型。
- **定價**：沿用現行 Claude Token 費率，無新定價。
- **文件**：https://platform.claude.com/docs/en/build-with-claude/message-threads
