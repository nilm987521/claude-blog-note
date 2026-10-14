---
title: "Uber's CISO on building an insider threat program for AI"
tags: [資安, AI代理人, 企業安全, 開源工具, 觀點]
createdAt: 2026-10-13
lastModified: 2026-10-14
---

## 文章資訊

- **來源**：Claude 部落格
- **網址**：https://claude.com/resources/articles/uber-s-ciso-on-building-an-insider-threat-program-for-ai
- **發布日期**：2026-10-13

## 重點摘要

1. **以員工內部威脅模型類比 AI 代理人監控**：Uber 資安長 Philip Martin 指出，AI 代理人的監控需求與企業內部員工威脅防護計畫本質相似，需要即時偵測與干預機制。

2. **前沿模型的進階威脅建模**：前沿大型語言模型能處理長情境資訊（包含程式碼、設計文件、Jira 歷史記錄），Martin 預見未來每個服務都可能配置能理解其威脅模型並跨代理人協作的 AI。

3. **Enterprise Frontier Safeguards 的資料主控權**：Uber 重視其資料在自身控制範圍內，未經許可不允許 Anthropic 存取；Uber 自行決定安全防護機制觸發後的應對措施。

4. **開源工具 ADR（AI Detection and Response）**：Uber 開源了 AI 偵測與回應工具，可收集即時遙測資料並在代理人執行框架內採取行動，能與 Anthropic 分類器的輸出整合，形成完整的 AI 使用監控防線。

5. **防禦者的兩大優先事項**：Martin 強調，近端即時偵測（貼近使用者提示詞）以及持續分析新興模型行為並將防護措施內建回平台，是企業 AI 安全的核心工作。

## 重要公告

- 本文章無新模型、新功能或價格變動等公告
- 文中強調 **Enterprise Frontier Safeguards** 功能，讓企業對 AI 活動保有完整的資料主控權
- Uber 的 **ADR 開源工具**可與 Anthropic 安全分類器結合使用，為 AI 代理人部署提供實務監控參考
