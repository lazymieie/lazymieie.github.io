---
title: "Generate Multiple Actions, Execute One: Experience-Guided Action Selection for LLM Agent Reinforcement Learning"
collection: publications
category: manuscripts
permalink: /publication/egas/
year: 2026
sort_order: 2
venue: "Manuscript · Under Review"
author_role: "First author"
selected: true
summary: "Expand candidate actions while executing a single trajectory, and reuse historical outcomes to train on both executed and unexecuted candidates."
share: false
comments: false
---

**Status:** Under review. **Contribution:** First author.

EGAS explores multiple candidate actions at each state while executing only one trajectory. A time-decayed posterior experience pool guides action selection, reducing the need to collect a separate continuation for every candidate.

Built on verl and GiGPO, the method combines experience-based advantage reweighting with an auxiliary pairwise preference objective. Historical execution outcomes provide training signals for candidates that are not executed in the current rollout.

Experiments cover ALFWorld, WebShop, and Sokoban using Qwen3-1.7B, Qwen3-4B, and Qwen3-VL-4B. The reported gains over GiGPO are **1.7–7.9 percentage points** in success rate, with **7.3%–25.0% fewer training trajectories** needed to reach the baseline's best performance.

<!-- Full author list and public paper/code URLs have not been supplied. -->
