---
title: "Comcast 和 Booz Allen 如何使用 Claude Mythos 發現漏洞鏈並保護程式碼庫"
tags: ["資安", "Claude Mythos", "企業案例", "漏洞偵測", "網路安全驗證計畫"]
createdAt: "2026-10-06"
lastModified: "2026-10-07"
---

## 文章資訊

**來源：** https://claude.com/resources/articles/how-comcast-booz-allen-use-claude-mythos-to-secure-their-codebases

## 重點摘要

1. **Claude Mythos 核心優勢**：Claude Mythos 擅長識別「漏洞鏈」——攻擊者串接多個輕微弱點的攻擊序列。與傳統工具只孤立分析單一漏洞不同，該模型能追蹤跨程式碼、設定和應用行為的相互關聯漏洞。

2. **Comcast 案例**：分析了 258 個業務關鍵系統及約 1.7 億行程式碼，Claude Mythos Preview 發現了一個橫跨多個相互作用元件的身份驗證繞過漏洞，是傳統方法無法偵測到的。其 CISO 指出：「發現速度越來越快……驗證這些龐大數量的發現才是新瓶頸。」

3. **Booz Allen 案例**：在 12 天內分析了橫跨 138 個儲存庫的 8 個正式環境系統，傳統方法需要數個月。發現了一個多層漏洞——一個橫跨兩個不同語言程式的未受保護安全金鑰，可讓攻擊者阻止裝置鎖定。

4. **人機協作不可或缺**：兩家組織都強調 AI 加速了發現過程，但人工驗證仍至關重要，團隊需要去重複化發現、確認可利用性並將問題分派給適當負責人。

5. **計畫背景**：此案例研究與 Anthropic 擴展網路安全驗證計畫（CVP）同步發布，為保護關鍵基礎設施的組織提供 Claude Mythos 模型存取權限。

## 重要公告

- **新模型：** Claude Mythos 已開放給通過網路安全驗證計畫（CVP）的組織使用
- 這是繼 Project Glasswing 之後，Anthropic 在企業資安領域的重大擴展
- 強調 AI 輔助資安的新瓶頸已從「發現」轉移至「驗證」階段
