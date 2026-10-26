---
title: "DEPPO: Dual Experience Pool Policy Optimization for Long-Horizon Reinforcement Learning"
collection: publications
category: conferences
permalink: /publication/deppo/
year: 2026
sort_order: 1
venue: "EMNLP 2026 · Main Conference"
author_role: "Co-first author"
paperurl: /files/DEPPO.pdf
selected: true
summary: "Step-level credit assignment from successful and failed historical trajectories, without an additional critic or process reward model."
share: false
comments: false
---

**Status:** Accepted to EMNLP 2026 (Main Conference). **Contribution:** Co-first author.

<a class="btn btn--primary" href="{{ page.paperurl | relative_url }}" download>Download paper (PDF)</a>

DEPPO addresses credit assignment in long-horizon agent tasks, where a terminal reward offers limited information about the contribution of intermediate actions.

The method maintains successful and failed experience pools indexed by task, state, and action. Smoothed action-conditional probability ratios estimate historical action preferences and reweight step-level advantages. Support constraints and weight clipping stabilize updates when historical observations are sparse.

The implementation builds on verl and GiGPO. On Qwen2.5-7B, the reported average success-rate gains over GiGPO are **7.1 percentage points on ALFWorld** and **9.1 percentage points on WebShop**, with additional evaluation on visual Sokoban.

<!-- Official author list and external publication/code URLs have not been supplied. -->
