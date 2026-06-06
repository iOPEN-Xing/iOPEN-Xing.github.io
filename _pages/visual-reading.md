---
title: "Visualized Reading"
permalink: /visual-reading/
layout: single
author_profile: true
excerpt: "论文与技术文章的可视化精读导航。"
---

{% include base_path %}

I turn papers and technical blogs I am actively reading into single-file, self-contained interactive HTML pages. Each entry below opens a standalone visual reading note; it is my way of forcing myself to restate the problem, method, evidence, and limitations in a form that someone else could also navigate.

这些页面不是摘要存档，而是“讲给别人听”的阅读笔记：尽量把论文的问题背景、解决动机、方法流程、关键图表和我的判断放在同一条叙事线上。

### [TokenSkip：让 CoT 可控变短，而不是事后硬截断]({{ base_path }}/files/visual-reading/tokenskip-cot-compression/)

<p class="page__meta">
  <time datetime="2026-06-06">Jun 6, 2026</time>
  · <span>paper</span>
  · <a href="https://arxiv.org/abs/2502.12067">original</a>
</p>

TokenSkip 讨论如何让 LLM 在保留推理能力的同时跳过 CoT 中低语义重要性的 token。阅读笔记重点梳理了问题背景、token importance 的训练信号、可控压缩率训练、与 prompt/truncation baseline 的差异，以及该方法在长 CoT 场景中的潜力与局限。
