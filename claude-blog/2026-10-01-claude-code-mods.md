---
title: "Customize Claude Code with mods"
tags: ["claude-code", "mods", "plugins", "customization", "typescript", "enterprise"]
createdAt: "2026-10-01"
lastModified: "2026-10-01"
---

# Customize Claude Code with mods

**文章網址：** https://claude.com/blog/claude-code-mods

## 重點摘要

1. **Mods 是什麼：** Anthropic 推出了「mods」功能，這是以 TypeScript 撰寫的小型函式，可以掛鉤（hook）到 Claude Code 的各個事件點，讓開發者無需等待官方功能發布即可自訂行為。

2. **核心能力：** Mods 能夠在提示詞送達模型前進行改寫、攔截或修改工具呼叫（封鎖、改寫、重試）、管理權限批准或拒絕請求、從工具輸出中遮蔽敏感資料，以及修改 UI 介面元素（新增自訂按鈕等）。

3. **企業應用場景：** 企業可利用 mods 實現 CI/CD 流水線狀態顯示、正式環境操作的確認防護機制，以及對所有 mod 互動的稽核日誌記錄，大幅增強了企業治理能力。

4. **安全機制：** Mods 隨 plugins 一起分發，遵循現有 plugin 控管規則。企業用戶有內建安全 mod `sec-default` 會優先載入，防止繞過權限規則等危險修改；但 mods 以完整機器權限執行、無沙盒隔離，應僅安裝來自可信來源的 mods。

5. **可用性：** 現已在 Claude Code CLI 與桌面版應用程式中提供，開發者可在 Claude 目錄中尋找現有 mods，或依照官方入門指南自行建立。

## 重要公告

- **新功能：Mods（自訂模組）** — Claude Code 正式引入 TypeScript-based 的 mods 系統，這是一項重大的可擴充性功能，讓開發者和企業能深度客製化 Claude Code 的行為與工作流程。
