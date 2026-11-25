---
title: "Turn artifacts into Mac and Windows apps"
tags: ["artifacts", "desktop-app", "beta", "mac", "windows"]
createdAt: 2026-11-24
lastModified: 2026-11-25
---

# Turn artifacts into Mac and Windows apps

**文章網址：** https://claude.com/resources/articles/install-as-app

## 重點摘要

1. **Artifact 可安裝為桌面應用程式（測試版）：** Claude 的 Artifact 現在可透過「Install as app」功能安裝為獨立的 Mac 或 Windows 桌面應用程式，擁有自己的圖示和視窗，不再侷限於 Claude 介面內。

2. **自動更新與連接器支援：** 安裝後的應用程式會隨 Artifact 更新而自動同步，同時可存取 Claude 和使用者已連接的連接器（使用量計入方案限額）。

3. **深度桌面整合：** 應用程式支援系統通知、選單列／系統匣項目，並可與桌面環境深度整合，提升使用體驗。

4. **三層權限設計：** 分為預設（僅瀏覽器等級）、App 權限（全螢幕、全域快捷鍵、通知等）和完整電腦存取（可執行程式、讀寫刪除檔案）三個層級；每次更新後需重新確認權限，確保安全性。

5. **使用限制與方案差異：** 目前適用於所有方案（HIPAA 合規組織與混合部署除外）；Team 方案預設開啟但關閉完整存取，Enterprise 方案需由管理員手動啟用；Claude Docs、Slides、Sheets 類型的 Artifact 暫不支援安裝。

## 重要公告

- **新功能：Artifacts 安裝為桌面應用程式（Beta）**，首批示範應用包含 Linnet（圖片編輯器）、Phosphor（檔案管理器）、Sift（資料夾整理）、Tern（終端機）、Vitals（效能監視器）。
- 無需額外打包、簽署、API 金鑰或單獨登入，只需透過 Share 選單中的「Install as app」即可完成安裝。
