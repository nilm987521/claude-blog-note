---
title: "給管理員更多 Claude 使用量的可見性與支出控管"
tags: [企業管理, 支出控管, 使用分析, Team, Enterprise, Admin, 計費]
createdAt: 2026-07-02
lastModified: 2026-07-02
---

## 文章網址

https://claude.com/blog/giving-admins-more-visibility-and-control-over-claude-spend

## 重點摘要

1. **成員層級分析即將預設開啟**：個人使用分析（Individual usage analytics）目前預設關閉，但自 2026 年 7 月 11 日起將改為預設開啟；若組織希望維持關閉狀態，需在該日期前後主動調整設定。
2. **多層級支出限額管理**：管理員可在三個層級設定支出上限——組織層級（organization）、群組層級（含角色型存取控制 RBAC）以及個人使用者層級，確保預算可預測且使用者保有彈性。
3. **細緻的使用數據可見性**：Team 和 Enterprise 計畫的管理員可查看成員依產品、模型、技能分類的詳細使用分析，並支援匯出 CSV 格式的每日更新支出報告（涵蓋每位使用者、每個模型的代幣用量與預估費用）。
4. **角色差異化權限**：Enterprise 計畫的 Admin 角色可查看所有分析（支出資料除外）；支出相關分析僅限 Owners 與 Primary Owners 存取，Team 計畫的 Owners 與 Primary Owners 亦可查看使用情況。
5. **程式化存取支援**：Enterprise Analytics API 提供程式化管道，可依代幣使用量或費用排列使用者清單，並依產品、模型、情境視窗或地區拆解使用趨勢與成本，適合大規模稽核與合規需求。

## 重要公告

- **隱私政策變更（7 月 11 日）**：成員層級使用分析將於 7 月 11 日預設開啟，組織管理員需提前評估是否要維持關閉，此為影響成員隱私的重要轉變。
- **三層支出控管架構**：新的組織 → 群組 → 個人層級支出限額體系，讓大型企業可精細化管控 AI 使用費用，避免預算超支。
- **Analytics API 增強**：Enterprise 方案提供程式化 Analytics API，可整合至內部 BI 或治理工具，強化企業對 Claude 用量的可稽核性。
