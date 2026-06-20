---
title: "Steering Claude Code：CLAUDE.md 檔案、技能、鉤子、規則、子代理全攻略"
tags: [Claude Code, CLAUDE.md, 技能, 鉤子, 子代理, 輸出樣式, 開發工具]
createdAt: 2026-06-19
lastModified: 2026-06-19
---

## 文章網址

https://claude.com/blog/steering-claude-code-skills-hooks-rules-subagents-and-more

## 重點摘要

1. **七種控制 Claude Code 行為的方法**：文章系統性介紹了 CLAUDE.md 檔案、規則（rules）、技能（skills）、子代理（subagents）、鉤子（hooks）、輸出樣式（output styles）以及附加系統提示（appending the system prompt）等七種指令方法，每種方法在「何時載入」、「是否跨壓縮持續存在」、「指令權重高低」三個維度上各有不同。

2. **CLAUDE.md 是長期設定的首選**：CLAUDE.md 放在專案根目錄，對話一開始便載入並貫穿整個 session，適合放置建構指令、目錄結構、monorepository 布局、程式碼慣例及團隊規範等固定資訊。

3. **技能 vs 子代理的使用時機**：當希望完整流程在主對話執行緒中展開、可以逐步觀察並調整時，選用技能（skill）；當側邊任務（如深度搜尋、日誌分析、相依性稽核）的中間結果不需要在主對話中顯示時，則改用子代理（subagent）以保持主對話簡潔。

4. **鉤子提供更確定性的行為控制**：鉤子是使用者定義的命令、HTTP 端點或 LLM 提示，在 Claude 生命週期的特定事件（檔案編輯、工具呼叫、session 啟動）觸發，相較於文字提示更具確定性、更不易受對話壓縮影響。

5. **輸出樣式擁有最高指令權重**：存放於 `.claude/output-styles/` 目錄的輸出樣式檔案，會注入系統提示，在所有方法中擁有最高的指令遵循優先級，適合強制要求特定格式或語調的場合。

## 重要公告

- **Claude Code 控制機制的完整指南**：此文章是 Anthropic 首次系統化公開說明開發者可用來客製化 Claude Code 行為的所有主要機制，對於想要在工程組織中大規模導入 Claude Code 的團隊具有重要參考價值。
- **明確的選擇決策框架**：文章提供了針對每種方法的適用場景指引，幫助開發者依照「希望指令何時生效」及「希望指令的持久程度」來選擇最適合的控制機制，降低試錯成本。
