---
title: "Introducing Claude Ship"
tags: ["claude-ship", "code-review", "pull-request", "ci", "enterprise", "新功能"]
createdAt: "2026-11-23"
lastModified: "2026-11-23"
---

## 文章資訊

**來源：** https://claude.com/resources/articles/introducing-claude-ship

## 重點摘要

- **Claude Ship 是什麼：** Anthropic 推出的全新系統，負責協助 Pull Request 的審查、修復與核准決策，目標是「讓程式碼和團隊撰寫速度一樣快地發布」。
- **程式碼審查（正式上線）：** 可從多個角度審查 PR、驗證發現的問題，並自動將審查結果發佈到 PR 上。團隊可針對每個 repo 選擇 Quick、Standard 或 Deep 三種審查等級。
- **PR Steward（測試版）：** 自動處理失敗的 CI 檢查、合併衝突與審查回饋，讓 PR 保持可合併狀態。每次推送後會留言說明變更內容，不會自行核准或合併。開發者可透過 `@claude` 指引方向，或以 `@claude stop` 中止。
- **Claude Approvals（測試版）：** 根據團隊撰寫並存放於 repo 中的核准政策運作，可自動核准例行性變更，或對特定情況要求人工簽核。建議先以「僅觀察模式」開始。
- **存取方式：** 開發者可在 Claude Code 中執行 `/ship` 指令，管理員可為整個 repo 啟用。適用於 Claude Team 與 Enterprise 方案的 GitHub repo，以 token 計費。**不支援** 零資料保留、HIPAA 設定或客戶自管加密金鑰的組織。

## 重要公告

- 推出全新 **Claude Ship** 產品，整合程式碼審查、PR 自動修復及核准流程
- **程式碼審查** 功能正式上線（GA），**PR Steward** 與 **Claude Approvals** 目前為測試版（beta）
