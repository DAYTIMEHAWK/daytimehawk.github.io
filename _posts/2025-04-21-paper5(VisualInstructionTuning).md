---
date: 2025-4-21
title: Visual Instruction Tuning
categories: [Literature Review]
tags: [微调]
---

### Background
使用机器生成的指令跟随数据(machine-generated instruction-following data)已经被证明能够在新任务上提升零样本能力，但是在多模态领域的探索还比较少，本文要将该思想引入多模态领域。

### Introduction
目前的
本文主要贡献：
1. 建立了多模态指令跟随数据(multimodal instruction-following data)：基于ChatGPT/GPT-4
2. 基于上述生成的数据进行指令微调(instruction-tuning)，构建了一个端对端训练的大型多模态模型(LMM)：`LLaVA`(Large Language and Vision Assistant)
   - `LLaVA`模型通过连接视觉编码器和语言解码器
   - `LLaVA`模型具有较好的多模态对话能力，在未见过的图像和指令上有时相对于`GPT-4`具有85.1%的相对得分
   - 在`Science QA`数据集上微调后，`LLaVA`和`GPT-4`协作达到了92.53%的高准确率
3. 开源，所有指令数据、代码等都是开源的

###