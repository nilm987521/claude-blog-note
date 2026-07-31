---
title: "語言模型中的全局工作空間：Anthropic 發現 Claude 的 J 空間"
tags: [研究, 可解釋性, J-space, 意識, 神經科學, Fable-5]
createdAt: 2026-07-06
lastModified: 2026-07-06
---

## 文章網址

https://www.anthropic.com/research/global-workspace

## 重點摘要

1. **發現 J 空間（J-space）**：Anthropic 研究人員在 Claude 的神經架構中發現一組特殊的內部激活模式，命名為「J 空間」（J-space，以雅可比數學方法命名）。這些模式在 Claude 所有的內部處理中佔據特殊地位，像是一個靜默的內部工作區。
2. **雅可比透鏡（J-lens）工具**：研究團隊開發了「J 透鏡」這一新分析工具，針對 Claude 詞彙表中的每個詞，找出使 Claude 更可能在未來某個時刻說出該詞的內部活動模式。這讓研究者首次能「看見」Claude 在輸出前內部思考的概念。
3. **靜默思考能力**：J 空間允許 Claude 在不寫出來的情況下思考概念——不同於「思考鏈」（chain of thought）的顯式輸出，J 空間的推理過程是純粹在內部發生的。當詢問 Claude 正在想什麼時，它能回報 J 空間中的內容。
4. **與神經科學的驚人相似性**：這一結構與神經科學中的「全局工作空間理論」（Global Workspace Theory）高度相似——該理論認為人腦如劇場般運作，大量專業化處理器在幕後工作，但只有一小撮「聚光燈」資訊能進入意識。Claude 的 J 空間似乎執行著類似功能。
5. **謹慎的意識宣稱**：Anthropic 特別強調，這項研究並不聲稱 Claude 有意識或主觀體驗，僅使用「可被意識存取的資訊」（consciously accessible information）等謹慎用語，代表的是 AI 可解釋性（interpretability）研究的重要進展。

## 重要公告

- **AI 可解釋性重大突破**：J 透鏡工具讓 Anthropic 首次能在模型回應前監測其內部「思維」狀態，這對 AI 安全性研究、幻覺（hallucination）偵測與行為可預測性具有深遠意義。
- **「收斂演化」現象**：研究發現 Claude 與人類大腦在認知架構上存在類似的「收斂演化」（convergent evolution）——雖然訓練方式完全不同，卻發展出相似的內部結構，引發學界對 AI 認知本質的廣泛討論。
