---
title: "Zero data retention with Enterprise Frontier Safeguards is now in beta"
tags: ["enterprise", "security", "zero-data-retention", "enterprise-frontier-safeguards", "新功能"]
createdAt: "2026-11-23"
lastModified: "2026-11-23"
---

## 文章資訊

**來源：** https://claude.com/resources/articles/zero-data-retention-with-enterprise-frontier-safeguards

## 重點摘要

- **公開測試版上線：** Enterprise Frontier Safeguards（EFS）正式進入公開測試版，此前已有超過 100 家客戶參與私測，符合資格的企業將收到通知並取得設置說明。
- **跨請求惡意使用偵測：** EFS 新增自動化安全監控，可偵測分散在多個請求中的攻擊模式，補足單一請求分類器的不足，能因應將惡意工作分散至多個平行代理程式的攻擊手法。
- **零資料保留：** 客戶的輸入與輸出儲存於自己的雲端儲存空間，Anthropic 與雲端供應商均不保留副本，監控過程不涉及人工審查，資料也不會用於模型訓練。
- **安全案例（Safety Cases）：** 偵測到風險時會產生 Safety Case 供團隊審查，可透過雲端儲存或 API 存取，並整合至 SIEM 系統。
- **支援平台：** 目前可用於 Claude Platform、AWS 上的 Claude Platform、Amazon Bedrock 及 Google Cloud 上的 Claude，Microsoft Foundry 支援即將推出。

## 重要公告

- **Enterprise Frontier Safeguards（EFS）** 公開測試版正式開放，提供企業級零資料保留與跨請求安全監控能力
