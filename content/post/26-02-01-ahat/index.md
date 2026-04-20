---
title: "Any House Any Task (AHAT) is Now Public"
date: 2026-02-01
authors:
  - zhihong
  - liyang
  - renming
  - Cewu Lu
  - panpan
---

🚀 Exciting News! We are thrilled to announce the release of our latest work:“Any House Any Task: Scalable Long-Horizon Planning for Abstract Human Tasks.” This research tackles long-horizon planning in large environments given ambiguous human instructions.

<!--more-->

## Paper Details

**Title:** Any House Any Task: Scalable Long-Horizon Planning for Abstract Human Tasks

**Authors:** Zhihong Liu, Yang Li, Renming Huang, Cewu Lu, Panpan Cai

**Abstract:** Open world language conditioned task planning is crucial for robots operating in large-scale household environments. While many recent works attempt to address this problem using Large Language Models (LLMs) via prompting or training, a key challenge remains scalability. Performance often degrades rapidly with increasing environment size, plan length, instruction ambiguity, and constraint complexity. In this work, we propose Any House Any Task (AHAT), a household task planner optimized for long-horizon planning in large environments given ambiguous human instructions. At its core, AHAT utilizes an LLM trained to map task instructions and textual scene graphs into grounded subgoals defined in the Planning Domain Definition Language (PDDL). These subgoals are subsequently solved to generate feasible and optimal long-horizon plans through explicit symbolic reasoning. To enhance the model's ability to decompose complex and ambiguous intentions, we introduce TGPO, a novel reinforcement learning algorithm that integrates external correction of intermediate reasoning traces into Group Relative Policy Optimization (GRPO). Experiments demonstrate that AHAT achieves significant performance gains over state-of-the-art prompting, planning, and learning methods, particularly in human-style household tasks characterized by brief instructions but requiring complex execution plans.

- **Paper**: [Available on arXiv](https://arxiv.org/abs/2602.12244)
- **Project Page**: [AHAT Project Website](https://sii-liyang2024.github.io/ahat/)

We are excited to share this work with the robotics community and look forward to your feedback and potential collaborations!
