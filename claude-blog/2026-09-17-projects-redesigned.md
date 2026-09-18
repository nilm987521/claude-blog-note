---
title: "Projects redesigned: from folder to conversation"
tags: [claude-code, agents, parallel-execution, projects, beta]
createdAt: 2026-09-17
lastModified: 2026-09-18
---

## 文章資訊

- **原文網址**：https://claude.com/blog/projects-redesigned
- **發布日期**：2026-09-17
- **來源**：Claude Blog

## 重點摘要

1. **Projects 架構全面重設計**：舊版 Projects 是「資料夾 + 單一對話」的形式，新版改為「協調者對話（coordinator conversation）+ 多執行緒（threads）」的平行代理架構，Claude 扮演工作協調者角色。

2. **自動化工作調度**：使用者只需描述目標，Claude 會自動拆解任務範疇、分派至各平行執行緒、協調進度、審查輸出，並整合最終結果，大幅降低手動協調成本。

3. **真正的雲端平行執行**：每個執行緒都是一個完整的 Claude Code 雲端工作階段，運行在獨立分支與獨立的儲存庫副本上，可平行同步進行，即使關閉電腦後仍持續執行。

4. **隨時隨地掌控進度**：使用者可透過手機等行動裝置隨時查看並介入調整進度，不需要守在電腦前，任務會在背景持續推進。

5. **Beta 公測開放**：本功能自 2026-09-17 起以 Beta 形式向部分 Claude Pro 與 Max 訂閱用戶開放，限定條件為有使用雲端工作階段且目前 Web/桌面版上無既有 Projects 的用戶。

## 重要公告

- **新功能發布**：Claude Code Projects 正式進入 Beta，核心功能是平行代理執行緒（parallel agent threads），這是 Claude Code 在大型工作協調上的重大升級。
- **適用對象**：Pro 及 Max 計畫的雲端工作階段用戶。
