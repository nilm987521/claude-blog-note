---
title: "How Block orchestrates Claude Fable across thousands of pull requests"
tags: [企業案例, Claude Fable, 程式碼遷移, 多代理架構]
createdAt: 2026-10-08
lastModified: 2026-10-09
---

## 文章資訊

- **來源**：Claude 部落格
- **網址**：https://claude.com/resources/articles/how-block-orchestrates-claude-fable-across-thousands-of-pull-requests
- **發布日期**：2026-10-08

## 重點摘要

1. **大規模程式碼遷移**：Block（Square、Cash App 母公司）利用 Claude Fable 進行全公司代碼庫遷移，可一次處理橫跨多個儲存庫的數百至數千個 Pull Request，突破過去模型單次僅能處理少數 PR 的限制。

2. **Claude Fable 擔任協調者（Orchestrator）**：Fable 負責高層次設計工作（資料模型、API 規格、演算法），再指揮數十個較小、成本較低的 Opus 或 Sonnet 模型執行檔案編輯與測試，由人類工程師監督整體流程。

3. **成本效益優化**：前沿模型（Fable）僅用於前期規劃，大多數代幣由較小模型負責，在不損失品質的前提下大幅降低成本；Block 正開發自動選擇器，依任務類型自動匹配最適模型與努力程度。

4. **工程角色轉變**：工程師的工作重心從機械式編程轉向遷移設計、代理行為審查及面向客戶的功能開發；Block 的「Buzz」開源工作空間讓人類與代理在共享頻道和執行緒中協作，提供遷移進度可見性。

5. **安全防護機制**：合併到主分支及正式環境部署需雙人簽核；代理的變更需通過安全檢查；Block 依賴 Fable 內建安全防護及 Anthropic 安全分類器，並已驗證 Claude 拒絕協助繞過雙重審批機制。

## 重要公告

- Block 的案例展示了 **Claude Fable 作為多代理協調者**的實際生產應用模式
- 此架構代表大型企業 AI 工程協作的新典範：AI 驅動大規模技術債清理與系統遷移
