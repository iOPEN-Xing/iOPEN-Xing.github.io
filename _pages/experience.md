---
title: "经历"
permalink: /experience/
author_profile: true
---

{% include base_path %}

## 美团

<img class="resume-org-logo" src="{{ base_path }}/images/meituan.png" alt="美团">

<p class="resume-meta"><strong>知识计算/智能交互部门，实习经历</strong><br>2025.11-2026.02</p>

### 基于快慢思考方式的外客在线主模型优化

<p class="resume-meta"><strong>技术点：</strong>冷启动数据工程、GRPO、SFT 退火模式融合</p>

- 针对传统客服大模型在复杂纠纷判责、资金退改等长链路推理场景中逻辑不连贯、幻觉率高且响应效率低等痛点，主导研发具备“快慢思考”能力的外客在线主模型。
- 在冷启动阶段，针对初期大规模蒸馏数据存在的逻辑发散与幻觉问题，重构冷启动策略，确立“高质量样本 + 模式化推理”的技术路线。
- 设计“知识增强与逆向 CoT 生成”范式，利用人工精标 Ground Truth 结合注入的业务规则，引导 SOTA 模型反向生成具备逻辑闭环的思维链；配合固定思维模板与严格的逻辑一致性质检，构建 8,000 条高信噪比垂直推理数据。
- 在强化学习阶段，利用 verl 框架落地 GRPO 算法，设计涵盖逻辑一致性及格式约束的多维奖励函数，提升模型判责准确性，并通过 SFT 退火机制实现模式融合。
- 上线后，知识增强单阶段 SFT 在方案准确率上提升 2.41pp，且优于双倍数据量的 SFT 对照组；快思考模式测试效果显著高于基线，平均首字延迟（TTFT）降低 40%。

### 基于生成式奖励模型的智能客服对齐与评估体系构建

<p class="resume-meta"><strong>技术点：</strong>非对称奖励函数、Reward Hacking Analysis</p>

- 针对即时配送客服场景中人工质检滞后及规则模型语义理解弱的痛点，主导构建基于 LongCat-18B 的生成式奖励模型，为强化学习中的 Policy 模型提供高置信度 RLHF 反馈。
- MVP 阶段通过 Zero-shot 验证快速识别 Reward Hacking、话术与方案不一致等问题，证伪纯 Prompt 路线。
- 架构升级阶段基于 REINFORCE++ 算法进行全参数训练，引入 BGE 语义约束与一致性校验，抑制过度询问倾向。
- 精细化调优阶段针对正样本主导导致的判别惰性，设计非对称奖励函数，通过重罚漏判机制实现高精度业务对齐。
- 最终，该 GRM 模型在正例场景下的判别一致性提升至 97% 左右，整体评估一致性达到 76.98%；接入该 GRM 进行 RLHF 训练后，客服策略模型的话术满分率达到 69.28%（优于基线 62.86%），方案正确率提升至 85.15%。

## 北京银行金融科技有限公司

<img class="resume-org-logo" src="{{ base_path }}/images/bank-of-beijing.png" alt="北京银行">

<p class="resume-meta"><strong>人工智能部门，实习经历</strong><br>2025.03-2025.06</p>

### 北银金融京脑 R1 大模型训练

<p class="resume-meta"><strong>技术点：</strong>金标蒸馏、裁判模型双轮质检、长文本一致性检验、GRPO</p>

- 为构建高质量 R1-Data 数据集，主导从数据构建到模型训练的全流程。
- 采用金标蒸馏技术，利用 DeepSeek 作为教师模型生成包含完整推理链的初始数据。
- 利用 Qwen2.5-72B-Instruct 作为裁判模型，从内部一致性、逻辑连贯性等七个关键维度进行双轮量化质检，提纯高质量训练样本。
- 在模型训练阶段，从 3w 条数据中选取 2.5w 条数据进行 SFT 微调；在模型后训练阶段，针对 1w 条数据采用 GRPO 算法进行强化学习。
- 编写“回答与真值语义一致性”优化奖励函数，通过任务类型分层识别、定制多维度校验规则，对答案进行精细化语义一致性判断，强化模型金融推理的稳定性和可解释性。
- GRPO 阶段使模型平均分比 SFT 后的模型平均提升 5% 左右；最终训练出的 BK-R1 模型在 FinQA 和 ConvFinQA 上取得 75.2 和 85.0 的 SOTA 分数。

## 中电信 TeleAI 研究院

<img class="resume-org-logo" src="{{ base_path }}/images/teleai.png" alt="中电信 TeleAI">

<p class="resume-meta"><strong>异构计算组，实习经历</strong><br>2024.11-2025.02</p>

### 基于 vLLM 框架使用 AutoAWQ 对 Telechat2 权重进行量化

- 针对 Telechat-2 模型因 KV 参数耦合存储无法直接量化注意力层的挑战，设计基于 vLLM 和 AutoAWQ 的混合量化方案。
- 通过重写底层接口并实施模块级阻断策略，将对量化鲁棒的 FFN 层（约占 2/3 参数）压缩至 INT8，同时强制保留高敏感度的 Attention 层为 FP16 精度。
- 该方案实现 W8A16 混合精度推理，在显著降低约 40% 显存占用的同时，将 MMLU、C-Eval 等基准测试的准确率损失控制在 1% 以内。
- 有效解决 Telechat2 大模型特殊架构下的量化部署难题。
