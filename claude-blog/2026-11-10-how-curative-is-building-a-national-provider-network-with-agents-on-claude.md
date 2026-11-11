---
title: "How Curative is building a national provider network with agents on Claude"
tags: ["客戶案例", "AI代理", "醫療保健", "多代理系統", "自動化"]
createdAt: "2026-11-10"
lastModified: "2026-11-10"
---

## 文章資訊

**原文網址：** https://claude.com/resources/articles/how-curative-is-building-a-national-provider-network-with-agents-on-claude

## 重點摘要

1. **Curative 與核心代理 Gwen**：Curative 是一家以零共付額、零自付額為主打的雇主健保公司，建立了核心代理 Gwen（使用 Claude Opus），負責從初次接觸到簽約的完整醫療提供者合約流程，每次執行皆獨立隔離，不保留跨交易資訊。
2. **多層代理審查機制**：使用 Sonnet 模型的費率審查代理可核准約三分之二超出標準費率範本的請求，剩餘非標準情況由 CEO 親自審核；Haiku 模型的「法官代理」在每封外寄訊息送出前進行審查，若被攔截則回傳原因讓 Gwen 修改。
3. **顯著成效**：Gwen 已簽署超過 23,000 份醫療提供者合約，每週達成 2,000 至 2,400 份（2025 年全年僅約 2,100 份）；每份合約成本降至原先的十分之一；合約爭議回應時間從 90 天縮短至 30 分鐘以內。
4. **工程師的 Claude Code 應用**：13 名工程師使用 Claude Code 重建了代理所運行的理賠、預先授權和財務系統，整個合約團隊從 45 人增至約 55 人，每人生產力提升約 2.5 倍。
5. **實踐心得與未來規劃**：關鍵經驗包括：單一通用工具優於多個專用工具、傳真管道將成約率倍增、以低風險場景先行測試後再處理受保護的健康資訊。Curative 計劃進一步新增會員護理導覽代理，並預期醫療提供者將部署自己的代理參與合約談判。

## 重要公告

無（此為客戶案例研究文章）
