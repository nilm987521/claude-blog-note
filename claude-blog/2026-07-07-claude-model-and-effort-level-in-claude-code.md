---
title: "Choosing a Claude model and effort level in Claude Code"
tags: [claude-code, model-selection, effort-level, productivity]
createdAt: 2026-07-07
lastModified: 2026-07-08
---

## 文章資訊

**網址：** https://claude.com/blog/claude-model-and-effort-level-in-claude-code  
**發布日期：** 2026-07-07

## 重點摘要

1. **模型選擇 vs. 努力等級有本質差異：** 模型選擇決定固定權重（整體能力範圍），努力等級則控制 Claude 完成請求的工作量，包含讀取的檔案數、使用的工具數量，以及回覆前執行的步驟數。

2. **努力等級不只是「思考時間」：** 高努力等級下，Claude 會在回覆前讀取更多檔案、執行測試並做自我確認；低努力等級下，Claude 傾向主動詢問更多背景資訊而非自行消耗 token 推算。

3. **選擇模型的判斷依據：** 常規任務使用較小模型，複雜或模糊的任務使用較大模型。若 Claude 明顯嘗試後仍得出錯誤答案，應升級至更強大的模型。

4. **選擇努力等級的判斷依據：** 若 Claude 犯錯原因是跳過了某個檔案、未執行測試，或中途放棄重構，這代表需要提高努力等級，而非更換模型。

5. **最佳實踐建議：** 從每個模型的預設努力等級開始使用，根據整體工作類型進行調整，無需針對每個任務逐一微調設定。

## 重要公告

無新模型或功能發布，此為 Claude Code 使用指引性文章，協助使用者更有效地搭配使用模型選擇與努力等級兩項設定。
