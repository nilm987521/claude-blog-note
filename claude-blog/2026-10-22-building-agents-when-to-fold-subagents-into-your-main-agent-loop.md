---
title: "Building agents: When to fold subagents into your main agent loop"
tags: ["agent", "subagent", "架構設計", "最佳實踐", "Claude"]
createdAt: "2026-10-22"
lastModified: "2026-10-22"
---

# 建構代理：何時將子代理整合進主代理迴圈

**文章網址：** https://claude.com/blog/building-agents-when-to-fold-subagents-into-your-main-agent-loop

## 重點摘要

1. **單一代理迴圈通常更有效**：在多家企業的實際部署比較中，搭配技能（skills）的單一代理，品質常優於「一個提示包辦所有任務」與「多子代理」兩種設計，且每項任務的成本與延遲通常較低。

2. **多子代理架構的常見問題**：情境在交接時流失、子代理數量失控、系統提示互相衝突、評估標準零散，以及整體延遲增加。

3. **漸進式揭露（Progressive Disclosure）**：技能與工具先只顯示簡短描述，需要時才完整載入，讓單一代理能處理多種任務，同時避免系統提示過長。

4. **仍應保留子代理的情境**：當單一迴圈出現可衡量的效能下降、需要平行處理並使用獨立情境視窗，或代理難以選擇工具、指令彼此衝突時，子代理仍有其價值。

5. **逐步遷移做法**：先建立端到端的評估集，再一次整合一個子代理，比較前後表現，只在單一迴圈表現較差時才保留子代理。

## 重要公告

- **新工具包**：Anthropic 發布 `single-agent-loop-kit`，協助開發者評估並遷移多代理系統至單一主迴圈架構。
- 文章提及 Opus 5.5 與 Fable 5.1 可在單一迴圈中處理更複雜的任務。
