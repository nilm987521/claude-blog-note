---
title: "Claude Fable 實戰指南：找出你的未知"
tags: [claude-fable, claude-code, 提示工程, 代理任務, 技巧, Fable-5]
createdAt: 2026-07-06
lastModified: 2026-07-06
---

## 文章網址

https://claude.com/blog/a-field-guide-to-claude-fable-finding-your-unknowns

## 重點摘要

1. **核心概念：地圖不等於疆域**：你給 Claude 的提示（地圖）與實際需要發生的工作（疆域）之間存在差距，稱為「未知」（unknowns）。Claude Fable 5 任務品質的瓶頸，不在模型本身，而在於你釐清未知的能力。
2. **四類未知框架**：作者將未知分成四類——已知的已知（known knowns）、已知的未知（known unknowns）、未知的已知（unknown knowns，你知道但忘記告訴 Claude 的事）、未知的未知（unknown unknowns，雙方都沒想到的事）。
3. **8 種揭露未知的技術**：跨越三個階段提供具體技術，包含實施前的「盲點分析」（blindspot passes）與「逆向訪談」（reverse interviews），實施中的「原始碼參考」（source-code references）與「實施筆記」（implementation notes），以及實施後的「測驗」（quizzes）等。
4. **Fable 5 的長時間代理能力**：Fable 5 可以自主運行數小時、觸及數十個檔案、端到端交付功能，這使得事前清晰定義未知比以往更為關鍵。
5. **廣泛迴響**：這篇由 Anthropic Claude Code 工程師 Thariq Shihipar 撰寫的指南，在發布後三天內獲得超過 200 萬次瀏覽，顯示業界對於如何有效使用 Fable 5 的強烈需求。

## 重要公告

- **提示工程典範轉移**：隨著 Claude Fable 5 具備長時間自主執行能力，傳統的「邊試邊改」提示方式已不足夠；在任務啟動前系統性地識別並消除未知，成為高品質代理任務的關鍵前置步驟。
- **實用技術框架**：這份指南提供可直接應用的具體技術（如讓 Claude 先進行盲點分析、反向訪談你以釐清需求），適合所有使用 Claude Code 或 Claude API 進行長時間代理任務的開發者參考。
