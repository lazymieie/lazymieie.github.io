---
layout: single
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume/
---
{% assign sorted_publications = site.publications | sort: 'sort_order' %}


## Education

**Fudan University** · Ph.D. Student, Electronic Information  
September 2026 — Present

**Wuhan University** · Bachelor’s Degree, Computer Science and Technology  
September 2022 — June 2026  
GPA: **3.971/4.0** · Rank: **1/231**

## Research Experience

**TeleAI** · Research Intern, Visual Understanding R&D Center  
November 2025 — August 2026

- PPO-based training and evaluation for long-horizon agents.
- Distributed MoE training with slime, Megatron, and SGLang.
- Segmented credit assignment, generalized advantage estimation, and reward reliability analysis.
- Agentic long-video understanding and vision encoder pretraining.

## Publications & Manuscripts

{% for publication in sorted_publications reversed %}
{% include publication-card.html publication=publication %}
{% endfor %}

## Research Projects

- Program evolution for embodied agents.
- State-level experience management and reinforcement learning.
- Agentic long-video understanding.
- Vision encoder pretraining.

[Project details]({{ '/projects/' | relative_url }})

## Honors & Awards

- **National Scholarship**, 2024 and 2025.
- **First-class Scholarship**, awarded in three undergraduate academic years.
- **Outstanding Student**, awarded in three undergraduate academic years.
- **Lei Jun Computer Science Undergraduate Scholarship**, 2023.
- **National Third Prize**, National College Student Computer System Capability Competition.
- Outstanding Youth League Member.
- Monthly Outstanding Intern recognition.

## Skills

- **Reinforcement Learning:** PPO, GRPO, credit assignment, and generalized advantage estimation (GAE).
- **Training Systems:** verl, slime, Megatron, SGLang, and distributed Mixture-of-Experts (MoE) training.
- **Agent Development:** tool-use harnesses, environment integration, reward validation, and experience management.
- **Multimodal & Embodied AI:** video understanding, vision encoder pretraining, and feedback-driven program evolution.

## Contact

[{{ site.author.email }}](mailto:{{ site.author.email }})
