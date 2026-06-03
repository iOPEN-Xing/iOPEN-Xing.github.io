---
permalink: /
title: "邢介政"
excerpt: "算法工程师候选人，关注 LLM post train、Agentic RL、Agentic 数据合成与 Agent 开发。"
author_profile: true
---

{% include base_path %}

我目前是西北工业大学光电与智能研究院智能科学与工程（计算机类）硕士生，本科毕业于大连海事大学智能科学与技术（计算机类）专业。求职方向为算法工程师，近期项目集中在 LLM post train、Agentic RL、Agentic 数据合成、生成式奖励模型与推理部署优化。

实习经历覆盖客服、金融和大模型推理部署场景：在美团参与外客在线主模型优化与智能客服奖励模型建设；在北京银行参与金融推理大模型 BK-R1 的数据构建、SFT 与 GRPO 后训练；在中电信 TeleAI 参与 Telechat2 的混合精度量化部署。整体上，我更关注如何把模型能力、数据质量、奖励设计和业务约束接起来，形成可验证的迭代闭环。

## 个人概览

<ul class="resume-facts">
  <li><strong>目标岗位：</strong>算法工程师</li>
  <li><strong>邮箱：</strong>jiezhengxing@gmail.com</li>
  <li><strong>电话：</strong>17709836681</li>
  <li><strong>籍贯：</strong>山东省济南市</li>
  <li><strong>硕士院校：</strong>西北工业大学</li>
  <li><strong>本科院校：</strong>大连海事大学</li>
</ul>

## 教育经历

<div class="resume-entry">
  <img class="resume-entry__logo" src="{{ base_path }}/images/npu-logo.png" alt="西北工业大学">
  <div>
    <h3>西北工业大学（“985 工程”）</h3>
    <p class="resume-meta"><strong>光电与智能研究院</strong><br>智能科学与工程（计算机类） · 2025.09-2028.06</p>
  </div>
</div>

<div class="resume-entry">
  <img class="resume-entry__logo" src="{{ base_path }}/images/dlmu-logo.png" alt="大连海事大学">
  <div>
    <h3>大连海事大学（“211 工程”）</h3>
    <p class="resume-meta"><strong>信息科学与技术学院</strong><br>智能科学与技术（计算机类） · 2021.09-2025.07</p>
    <ul>
      <li>成绩排名：前 8%；单学期最高 GPA：4.56</li>
      <li>荣誉：优秀学生奖学金、辽宁省竞赛奖学金、校优秀毕业生</li>
    </ul>
  </div>
</div>

## 感兴趣方向

- LLM post train
- Agentic RL
- Agentic 数据合成
- Agent 开发

## 竞赛经历

<ul class="resume-competition-list">
  <li><span>2026</span><strong>华为杯软件挑战赛</strong><span>西北赛区二等奖</span></li>
  <li><span>2025</span><strong>华为杯数学建模研究生大赛</strong><span>全国二等奖</span></li>
  <li><span>2024</span><strong>全国大学生数学建模大赛</strong><span>全国二等奖</span></li>
  <li><span>2024</span><strong>机器人与人工智能大赛</strong><span>全国二等奖</span></li>
  <li><span>2024</span><strong>百度之星程序设计大赛</strong><span>辽宁省铜奖</span></li>
</ul>

## 经历摘要

<div class="resume-company-entry">
  <div class="resume-company-heading">
    <img src="{{ base_path }}/images/meituan.png" alt="美团">
    <h3>美团，知识计算/智能交互部门</h3>
  </div>
  <p class="resume-meta"><strong>实习经历</strong> · 2025.11-2026.02<br><strong>核心技术：</strong>冷启动数据工程、逆向 CoT、GRPO、verl、SFT 退火、生成式奖励模型、REINFORCE++、BGE 语义约束</p>
  <ul>
    <li>面向外客在线客服中的复杂纠纷判责、资金退改等长链路推理场景，主导优化具备“快慢思考”能力的在线主模型。通过知识增强与逆向 CoT 生成构建 8,000 条高信噪比垂直推理数据，并结合 GRPO 奖励设计和 SFT 退火完成模式融合；知识增强单阶段 SFT 使方案准确率提升 2.41pp，快思考模式 TTFT 降低 40%。</li>
    <li>面向即时配送客服中人工质检滞后、规则模型语义理解弱的问题，构建基于 LongCat-18B 的生成式奖励模型，为 Policy 模型提供 RLHF 反馈。通过 Zero-shot 验证定位 Reward Hacking，后续引入 REINFORCE++、BGE 语义约束与非对称奖励函数；GRM 正例判别一致性提升至 97% 左右，整体评估一致性达到 76.98%，接入后策略模型话术满分率达到 69.28%，方案正确率提升至 85.15%。</li>
  </ul>
</div>

<div class="resume-company-entry">
  <div class="resume-company-heading">
    <img src="{{ base_path }}/images/bank-of-beijing.png" alt="北京银行">
    <h3>北京银行金融科技有限公司，人工智能部门</h3>
  </div>
  <p class="resume-meta"><strong>实习经历</strong> · 2025.03-2025.06<br><strong>核心技术：</strong>金标蒸馏、裁判模型双轮质检、长文本一致性检验、SFT、GRPO、金融语义一致性奖励函数</p>
  <ul>
    <li>面向金融问答和多轮推理场景，参与北银金融京脑 R1 大模型训练，负责从 R1-Data 数据构建到模型训练的关键环节。通过 DeepSeek 金标蒸馏生成推理链数据，使用 Qwen2.5-72B-Instruct 从内部一致性、逻辑连贯性等七个维度进行双轮质检，并在 2.5w 条数据上完成 SFT、1w 条数据上进行 GRPO 后训练；GRPO 阶段较 SFT 后平均分提升 5% 左右，BK-R1 在 FinQA 和 ConvFinQA 上取得 75.2 和 85.0 的 SOTA 分数。</li>
  </ul>
</div>

<div class="resume-company-entry">
  <div class="resume-company-heading">
    <img src="{{ base_path }}/images/teleai.png" alt="中电信 TeleAI">
    <h3>中电信 TeleAI 研究院，异构计算组</h3>
  </div>
  <p class="resume-meta"><strong>实习经历</strong> · 2024.11-2025.02<br><strong>核心技术：</strong>vLLM、AutoAWQ、W8A16、INT8/FP16 混合精度、MMLU、C-Eval</p>
  <ul>
    <li>面向 Telechat2 特殊架构下 KV 参数耦合导致注意力层难以直接量化的问题，设计基于 vLLM 与 AutoAWQ 的混合量化方案。通过重写底层接口和模块级阻断策略，将 FFN 层压缩至 INT8，同时保留 Attention 层 FP16 精度，实现 W8A16 混合精度推理；显存占用降低约 40%，MMLU、C-Eval 等基准测试准确率损失控制在 1% 以内。</li>
  </ul>
</div>

## 待补充信息

- GitHub / 个人主页：***
- 论文 / 专利 / 开源项目：***
- 政治面貌完整字段：中共预备***
