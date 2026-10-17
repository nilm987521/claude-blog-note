---
title: "How an Anthropic Japan BDR runs his day with a fleet of Claude agents"
tags: ["Claude Managed Agents", "Claude Tag", "最佳實踐", "業務開發", "自動化", "工作流程"]
createdAt: "2026-10-16"
lastModified: "2026-10-16"
---

# How an Anthropic Japan BDR runs his day with a fleet of Claude agents

**文章網址：** https://claude.com/resources/articles/how-an-anthropic-japan-business-development-representative-runs-his-day

## 重點摘要

1. **六代理人艦隊自動化日常業務工作：** Anthropic 日本業務開發代表 Shahboz Ibragimov 建立了六個 Claude 代理人，各有日文名稱——Furiwake（潛在客戶路由）、Sabaki（資格審核與首次聯繫郵件）、Henji（回覆客戶郵件）、Shoudan（維護 Salesforce 紀錄）、Nokori（會議摘要與後續行動跟進），以及一個協調代理人負責更新其他代理人的指令；整套系統每週為他節省約 60 小時工作量。

2. **Claude Managed Agents 統一管理：** 原先需在多個聊天視窗分散管理技能、排程任務和資料夾，遷移至 Claude Managed Agents 後可在單一介面集中管理，並支援版本化指令、共享記憶體庫及憑證保管庫；每個代理人僅獲得其工作所需的最低存取權限。

3. **跨代理人學習機制：** 所有代理人共享同一記憶庫，透過比較草稿與實際發送郵件的差異持續學習優化；一次修正可跨整個代理人艦隊生效，無需逐一調整。

4. **Claude Tag 整合 Slack 工作流程：** 需要進一步跟進的事項會交由 Claude Tag 處理，Claude Tag 在 Slack 討論串中自行設定提醒，並在需要人工審核時標記作者，實現非同步的人機協作。

5. **依任務複雜度選用模型：** Furiwake 和 Shoudan 使用 Sonnet，Sabaki、Nokori 和協調代理人使用 Opus，Henji 使用 Sonnet 並透過「顧問策略（advisor strategy）」在遇到困難決策時諮詢 Opus，兼顧成本與品質。

## 重要公告

- **Claude Managed Agents（測試版）：** Anthropic 推出代理人管理基礎設施，提供排程部署、共享記憶體庫、版本化指令及管理憑證保管庫，可透過 Console 快速啟動範本開始使用。
- **Claude Tag（測試版）：** Claude 可作為 Slack 工作空間成員加入，接收標記後在討論串中處理任務並自動設定後續提醒。
- **顧問策略（Advisor Strategy）：** 新的多模型協作模式，由較小模型執行任務，遇到困難決策時自動諮詢較大模型，在效能與成本之間取得平衡。
