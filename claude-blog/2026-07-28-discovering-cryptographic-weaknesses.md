---
title: "Discovering cryptographic weaknesses with Claude"
tags:
  - research
  - cryptography
  - security
  - claude-mythos
  - HAWK
  - AES
  - post-quantum
createdAt: 2026-07-28
lastModified: 2026-07-28
---

## 文章資訊

**網址：** https://www.anthropic.com/research/discovering-cryptographic-weaknesses

## 重點摘要

1. **Claude Mythos Preview 協助發現加密弱點**：Anthropic 研究人員借助 Claude Mythos Preview 在兩種加密算法中找到了安全弱點——這些弱點在多年的人類專家審查中都未被發現。

2. **HAWK 後量子簽名方案遭弱化**：Claude 在僅約 60 小時的工作量下改進了針對 HAWK（一種為後量子時代設計的數位簽章方案）的最佳已知攻擊，有效將其密鑰安全強度削減一半；而 HAWK 此前已通過兩年、兩輪的專家人工審查。

3. **AES 縮減版攻擊效率大幅提升**：研究人員同時改進了針對 AES 7 輪縮減研究版本的攻擊，效率提升達 200–800 倍。

4. **多代理研究系統執行**：整個研究過程由具備數學軟體、已發表論文和計算工具存取權限的多代理系統完成，人類研究員僅偶爾提供指導，且不具備格基密碼學的專業知識。研究耗資約 10 萬美元的 API 用量。

5. **目前不影響生產系統**：兩項發現均不構成立即風險——HAWK 尚未部署於生產環境，而 AES 攻擊僅適用於七輪縮減研究版本，而非完整的十輪 AES-128 加密。

## 重要公告

- **前沿 AI 輔助密碼學研究**：這是 AI 系統首次在一般密碼學研究中達到、甚至超越頂尖人類專家水準的具體案例，顯示 Claude Mythos 在科學研究領域的強大能力。
- **研究成本僅需 10 萬美元**：以 AI 代理完成原本需要專家團隊數年的研究，展現 AI 在降低高度專業化研究成本方面的潛力。
