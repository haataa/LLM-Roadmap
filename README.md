# Overview
This project is dedicated to curating, organizing, and sharing the latest research developments, papers, and resources in the field of Large Language Models (LLMs). My goal is to create a comprehensive repository that serves as a valuable resource for researchers, practitioners, and enthusiasts interested in the advancements and applications of LLMs.

# Contents
- [Typical LLMs](#Typical-LLMs)
- [Pretrain Method](#Pretrain-Method)
- [Instruction Finetune](#Instruction-Finetune)
- [Prompt Engineer](#Prompt-Engineer)
- [PEFT](#PEFT)
- [Compression](#Compression)
- [Extent Length](#Extent-Length)
- [RAG](#RAG)


# Typical LLMs
## Instruct GPT
- **Paper**:[Training language models to follow instructions with human feedback](https://arxiv.org/pdf/2203.02155.pdf)
- **year**:2022/02
- **summary/reason to read**: must-read paper from openai
## llama
- **Paper**:[LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/pdf/2302.13971.pdf)
- **year**:2023/02
- **summary/reason to read**: most widely used opensource llms now
## llama2
- **Paper**:[https://arxiv.org/pdf/2307.09288.pdf](https://arxiv.org/pdf/2307.09288.pdf)
- **year**:2023/07
- **summary/reason to read**: most widely used opensource llms now
## Mamba
- **Paper**:[Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/ftp/arxiv/papers/2312/2312.00752.pdf)
- **year**:2023/12
- **summary/reason to read**: potential archetecture to replace transformers
## Jamba
- **Paper**:[Jamba:A Hybrid Transformer-Mamba Language Model](https://arxiv.org/pdf/2403.19887.pdf)
- **year**:2024/03
- **summary/reason to read**: [混合了Transformer和Mamba层以及MoE组件的混合框架LLM](https://www.xiaohongshu.com/explore/660baf16000000001a00fa86)
## DeepSeek-Coder-v2
- **Paper**:[DeepSeek-Coder-V2: Breaking the Barrier of Closed-Source Models in Code Intelligence](https://arxiv.org/pdf/2406.11931)
- **year**:2024/06
- **summary/reason to read**: [最佳开源coding模型](https://www.xiaohongshu.com/explore/667a8fbe000000001e013a8a?xsec_token=ABxBQz-sXlkOedu_Dk8-8Eieh9bO6zttFzVXEEtj9iznw=&xsec_source=pc_user)
# Surveys
# Pretrain Method
## system
### DeepSpeed ZeRO
- **Paper**:[ZeRO: Memory Optimizations Toward Training Trillion Parameter Models](https://arxiv.org/pdf/1910.02054.pdf)
- **year**:2019/10
- **summary/reason to read**: commonly used pretrain framework
# MOE
# Instruction Finetune
- **Paper**:[Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2203.02155.pdf)
- **year**:2022/03
- **summary/reason to read**: 最早讲instruct finetune的论文之一
# RLHF
## DPO
- **Paper**:[Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/pdf/2305.18290.pdf)
- **year**:2023/05
- **summary/reason to read**: [使用变量变换将奖励函数上的损失函数转化为直接基于策略的损失函数从而无需训练reward function](https://www.xiaohongshu.com/explore/65782f9a0000000016007f93)
## KTO
- **Paper**:[KTO: Model Alignment as Prospect Theoretic Optimization](https://arxiv.org/pdf/2402.01306.pdf)
- **year**:2024/02
- **summary/reason to read**: [使用相对偏好数据最大化LLM生成效用来对齐模型](https://www.xiaohongshu.com/explore/6583ea850000000038022997)
## SPPO
- **Paper**:[Self-Play Preference Optimization for Language Model Alignment](https://arxiv.org/pdf/2405.00675)
- **year**:2024/05
- **summary/reason to read**: [使用博弈论对LLM进行强化学习](https://www.xiaohongshu.com/explore/6639ebe3000000001e033ea1)
# Prompt Engineer
# PEFT
## Lora
- **Paper**:[LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODEL](https://arxiv.org/pdf/2106.09685.pdf)
- **year**:2021/06
- **summary/reason to read**:目前最常用的PEFT方法
## Towards a Unified View of Parameter-Efficient Transfer Learning
- **Paper**:[Towards a Unified View of Parameter-Efficient Transfer Learning](https://arxiv.org/pdf/2110.04366.pdf)
- **year**:2021/10
- **summary/reason to read**:用统一的视角分析了所有PEFT方法
## Lora+
- **Paper**:[LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf)
- **year**:2024/02
- **summary/reason to read**:[给LoRA的两个矩阵分配不同的学习率，LoRA的效果还能进一步提升](https://kexue.fm/archives/10001)
## Dora
- **Paper**:[DoRA: Weight-Decomposed Low-Rank Adaptation](https://arxiv.org/pdf/2402.09353.pdf)
- **year**:2024/02
- **summary/reason to read**:[将预训练权重分解为振幅和方向两部分进行微调](https://www.xiaohongshu.com/explore/65d30eb8000000000102a1f8)
## ReFT
- **Paper**:[ReFT: Representation Finetuning for Language Models](https://arxiv.org/pdf/2404.03592.pdf)
- **year**:2024/04
- **summary/reason to read**:[修改隐藏层表征来进行微调参数效率提高10倍](https://www.xiaohongshu.com/explore/66164f2c000000001a0145c1)
# Extent Length
## Position Interpolation
- **Paper**:[EXTENDING CONTEXT WINDOW OF LARGE LANGUAGE MODELS VIA POSITION INTERPOLATION](https://arxiv.org/pdf/2306.15595.pdf)
- **year**:2023/06
- **summary/reason to read**: 线性外插的方法拓展长度
## Attention Based
- **Paper**:[LM-INFINITE: SIMPLE ON-THE-FLY LENGTH GENERALIZATION FOR LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2308.16137.pdf)
- **year**:2023/08
- **summary/reason to read**:[Lambda-shaped 注意力掩码和距离限制](https://www.xiaohongshu.com/explore/64fe8cb7000000001e021ec5)
## Fine-tuning based
- **Paper**:[LONGLORA: EFFICIENT FINE-TUNING OF LONGCONTEXT LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2309.12307.pdf)
- **year**:2023/09
- **summary/reason to read**:[使用Shift Short Attention技术在保持原始模型架构不变的情况下扩展模型的上下文窗口](https://www.xiaohongshu.com/explore/6511556f000000001d016c8c)
# Compression
## Pruning
### SLICEGPT
- **Paper**:[SLICEGPT: COMPRESS LARGE LANGUAGE MODELS BY DELETING ROWS AND COLUMNS](https://arxiv.org/pdf/2401.15024.pdf)
- **year**:2024/01
- **summary/reason to read**:[通过删除大型语言模型中的行和列来实现模型的压缩](https://www.xiaohongshu.com/explore/65ba158a0000000008020723)
### ShortGPT
- **Paper**:[ShortGPT: Layers in Large Language Models are More Redundant Than You Expect](https://arxiv.org/pdf/2403.03853.pdf)
- **year**:2024/03
- **summary/reason to read**:[LLMs中的许多层存在高度相似性根据BI分数直接删除冗余层](https://www.xiaohongshu.com/explore/660a6784000000001a0109d8)
### The Unreasonable Ineffectiveness of the Deeper Layers
- **Paper**:[The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/pdf/2403.17887.pdf)
- **year**:2024/03
- **summary/reason to read**:[计算不同层之间的相似性来剪枝并通过微调来修复性能损失](https://www.xiaohongshu.com/explore/660a6784000000001a0109d8)
## Quantization
### 基础知识
- **blog**:[目前针对大模型进行量化的方法有哪些？](https://www.zhihu.com/question/627484732/answer/3261671478)
### Quantization-Aware Fine-tuning(QAF)
#### QLORA
- **Paper**:[QLORA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/pdf/2305.14314.pdf)
- **year**:2023/05
- **summary/reason to read**::通过一个冻结的4位量化的预训练语言模型反向传播梯度进行Lora训练
#### QA-LORA
 - **Paper**:[QA-LORA: QUANTIZATION-AWARE LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/pdf/2309.14717.pdf)
 - **year**:2023/09
 - **summary/reason to read**:[通过组操作增加低位量化的自由度同时减少适应的自由度实现量化感知的Lora训练](https://www.xiaohongshu.com/explore/652e4fbb000000001e022e99)
 ### Post Training Quantization(PTQ)
 #### GPTQ
 - **Paper**:[GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/pdf/2210.17323.pdf)
 - **year**:2022/10
 #### AWQ
 - **Paper**:[AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration](https://arxiv.org/pdf/2306.00978.pdf)
 - **year**:2023/10
# MultiModa
# Agent
## surveys
### AI AGENT Cognitive Architectures
- **Paper**:[Cognitive Architectures for Language Agents](https://arxiv.org/pdf/2309.02427)
 - **year**:2023/09
### AI AGENT ARCHITECTURES
- **Paper**:[THE LANDSCAPE OF EMERGING AI AGENT ARCHITECTURES FOR REASONING, PLANNING, AND TOOL CALLING: A SURVEY](https://arxiv.org/pdf/2404.11584)
 - **year**:2024/02
### Multi-Agents
- **Paper**:[Large Language Model based Multi-Agents: A Survey of Progress and Challenges](https://arxiv.org/pdf/2402.01680v1)
 - **year**:2024/02
# RAG
## LongLLM vs RAG
- **Paper**:[Can Long-Context Language Models Subsume Retrieval, RAG, SQL, and More?](https://arxiv.org/pdf/2406.13121)
- **year**:2024/06
## LongRAG
- **Paper**:[LongRAG: Enhancing Retrieval-Augmented Generation with Long-context LLMs](https://arxiv.org/pdf/2406.15319)
- **year**:2024/06

# Domain Usage
