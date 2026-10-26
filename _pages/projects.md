---
layout: single
title: "Research Projects"
permalink: /projects/
author_profile: true
---

## Program Evolution for Embodied Agents

<p class="project-period">October 2026</p>

Developed a self-improving system that represents embodied manipulation policies as executable programs. An offline loop localizes errors, diagnoses failures, repairs code, and validates changes in simulation. Repair cases become reusable skills, while online agent assistance supports recovery when execution stalls.

On LIBERO-PRO, the reported program-library success rate increases from **20% to 89.47% without model calls at execution time**, reaching **95.80% with online Astra recovery**.

## PPO-based Agentic RL

<p class="project-period">May — July 2026 · TeleAI</p>

Adapted training environments and optimized PPO workflows for long-horizon, multi-turn tool use. Set up a **24-GPU, 3-node** training workflow for **Qwen3-30B-A3B** using slime, Megatron, and SGLang, with tensor, context, and expert parallelism.

Integrated BFCL multi-turn environments and task execution/reward interfaces for QwenClawBench. Implemented segmented PPO with segment-level generalized advantage estimation and critic losses at segment boundaries. The reported BFCL Multi-Turn-Base success rate is **73%**.

## State-level Experience Management

<p class="project-period">March — May 2026</p>

Designed an agentic harness for state-level experience storage and on-demand retrieval. Combined experience-guided rollouts with GRPO training to support policy improvement.

## Agentic Long-video Understanding

<p class="project-period">TeleAI Internship</p>

Built a multi-turn harness with tools for global video overviews, segment localization, and local verification, enabling task-driven exploration and evidence localization in long videos.

## Vision Encoder Pretraining

<p class="project-period">TeleAI Internship</p>

Worked on vision encoder pretraining and integration of billion-scale image–text data. Combined global contrastive learning with generative caption learning to improve semantic alignment and fine-grained visual representations.
