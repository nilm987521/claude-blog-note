---
title: "How Anthropic runs large-scale code migrations with Claude Code"
tags:
  - claude-code
  - code-migration
  - dynamic-workflows
  - enterprise
  - opus-4-8
createdAt: "2026-07-16"
lastModified: "2026-07-17"
---

## 文章資訊

- **來源**：[How Anthropic runs large-scale code migrations with Claude Code](https://claude.com/blog/how-anthropic-runs-large-scale-code-migrations-with-claude-code)
- **發布日期**：2026-07-16
- **分類**：Claude Code

## 重點摘要

1. **動態工作流程（Dynamic Workflows）驅動大規模遷移**：Anthropic 在 Claude Code 中使用動態工作流程，讓 Claude 自動生成協調腳本，在單一會話中啟動數十至數百個平行子代理，處理橫跨數百甚至數千個檔案的大型程式碼遷移任務。

2. **內建驗證機制**：工作流程在合併結果前會由獨立代理進行檢查或反駁，確保程式碼品質。整個流程以現有測試套件作為完成標準，把驗證從開發者手動確認轉為自動化仲裁。

3. **真實案例：Bun 從 Zig 移植至 Rust**：Bun 執行環境團隊透過動態工作流程，在 11 天內將約 75 萬行程式碼從 Zig 移植到 Rust，並保持 99.8% 的既有測試套件通過率，完整示範了此工具在超大規模遷移中的實用性。

4. **可中斷後續接工作**：執行過程中進度會持續儲存，若任務中途中斷，下次啟動時可從中斷點繼續，不需從頭重來，大幅降低風險。

5. **方案支援範圍**：動態工作流程在 Max、Team、Enterprise 方案及 API 上預設啟用；Pro 方案使用者可在 `/config` 中手動開啟。此功能會消耗比一般 Claude Code 會話更多的用量。

## 重要公告

- Claude Code 搭配 Opus 4.8 現可端對端執行整個程式碼庫規模的遷移，從啟動到合併 pull request 全程自動化。
- 此篇文章以 Anthropic 自身如何在內部應用 Claude Code 進行程式碼遷移作為實例，具有高度參考價值。
