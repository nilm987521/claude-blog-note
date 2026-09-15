---
title: "Agentic coding is straining CI. Here's how we scaled test impact analysis at Anthropic"
tags: [工程實踐, CI/CD, 代理程式碼, 測試基礎設施, 可擴展性]
createdAt: 2026-09-14
lastModified: 2026-09-14
---

## 文章資訊

- **網址**：https://claude.com/blog/agentic-coding-is-straining-ci-heres-how-we-scaled-test-impact-analysis-at-anthropic
- **發布日期**：2026-09-14
- **作者**：Sachin Malhotra

## 重點摘要

1. **程式碼產量爆炸性成長**：Anthropic 工程師每季平均交付的程式碼量是 2021–2025 年的 8 倍，其中 Claude 撰寫了 80% 的程式碼，並大量參與 PR 審查與核准。

2. **CI 成為新瓶頸**：寫程式已不再是主要約束，當 PR 審查也被加速後，持續整合（CI）開始承受巨大壓力——六個月內 CI 任務增加了 25 倍，測試數量成長了 10 倍。

3. **測試影響分析服務瀕臨崩潰**：規模的急劇擴張導致 Anthropic 的測試影響分析服務多次面臨過載危機，最終迫使團隊完全拆解並重新設計服務架構。

4. **重新設計為水平擴展架構**：新架構採用水平擴展設計，能夠應對代理程式碼生成所帶來的爆炸性工作量成長，確保 CI 管線的穩定性。

5. **行業趨勢預警**：Anthropic 指出，隨著代理持續加速程式碼生成，越來越多的工程團隊將面臨相同挑戰，水平擴展的測試選擇架構可能很快成為業界標準。

## 重要公告

- **工程實踐啟示**：這篇文章揭示了 AI 驅動開發（即「vibe coding」/代理編程）對工程基礎設施帶來的實際且深刻的衝擊，提供了 Anthropic 內部應對 CI 規模挑戰的第一手技術案例，具有重要的行業參考價值。
