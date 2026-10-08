---
title: "Automating eval design and hillclimbing with Claude"
tags: ["eval", "hillclimbing", "claude-api", "claude-code", "評估", "自動化"]
createdAt: "2026-10-07"
lastModified: "2026-10-07"
---

## 文章資訊

**來源：** https://claude.dev/blog/automating-eval-design-and-hillclimbing/
**發布日期：** 2026-10-07

## 重點摘要

1. **自動建立評估套件**：`/claude-api build-eval` 指令讓 Claude 與開發者進行互動訪談，自動在程式碼庫中建立評估套件；輸入樣本依優先順序取自生產記錄、錯誤報告或合成案例，並建立可靠的評分器（程式化檢查或具可驗證評分標準的 LLM 評審）。

2. **自動 hillclimbing 迭代優化**：`/claude-api hillclimb` 指令將評估集隨機分為訓練組與測試組，透過反覆迭代尋找最佳系統提示或設定；只保留兩組分數同時提升的變更，訓練組提升但測試組持平則視為過度擬合並還原，確保優化具有泛化能力。

3. **成本與效能雙提升**：實際案例顯示，客服票務系統準確率從 78.6% 提升至 90.5%，成本降低約 5 倍；另一案例從 Opus 4.8（74.4% 準確率，每票 $0.046）優化至 Sonnet 5（98.9% 準確率，成本約五分之一）。

4. **內建過度擬合防護**：分割評估集的設計確保模型不會只針對訓練範例調整；建議生產部署使用至少 50 個案例，每個配置至少執行 5 次以確保結果穩定性。

5. **與 Claude Code 整合**：功能於 Claude Code 2.1.259 版本起提供，作為 `/claude-api` skill 的一部分，適用於任何使用 Anthropic API 的應用程式開發工作流程。

## 重要公告

- **新工具發布**：`/claude-api build-eval` 與 `/claude-api hillclimb` 指令可大幅簡化 AI 應用的評估與優化流程
- **最低版本要求**：需要 Claude Code 2.1.259 或更新版本
