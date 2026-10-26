---
permalink: /
title: "Jiaxin Guo <span class='name-cn'>郭嘉欣</span>"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
{% assign sorted_publications = site.publications | sort: 'sort_order' %}


<p class="intro-kicker">Ph.D. Student · Fudan University</p>

I am a Ph.D. student in Electronic Information at **Fudan University**. Previously, I received my bachelor’s degree in Computer Science and Technology from **Wuhan University**, where I ranked **1st out of 231** students with a GPA of **3.971/4.0**.

My research focuses on **reinforcement learning for LLM agents**, especially credit assignment, experience reuse, and efficient exploration in long-horizon tasks. I am also interested in coding agents and embodied intelligence: how agents can turn execution feedback into reusable programs and skills.

I previously interned at **TeleAI**, working on agentic RL, agentic long-video understanding, and vision encoder pretraining.

<div class="profile-links">
  <a class="profile-link-primary" href="mailto:{{ site.author.email }}"><i class="fas fa-envelope" aria-hidden="true"></i> Get in touch</a>
  <a href="#publications">Publications <span aria-hidden="true">↓</span></a>
  <a href="#cv">Curriculum vitae <span aria-hidden="true">↓</span></a>
</div>

## Research Interests

<ul class="research-interests">
  <li><strong>Agentic Reinforcement Learning</strong><span>Long-horizon credit assignment and reliable policy optimization.</span></li>
  <li><strong>Experience and Exploration</strong><span>Learning from historical trajectories and action candidates.</span></li>
  <li><strong>Coding and Embodied Agents</strong><span>Program evolution, reusable skills, and feedback-driven improvement.</span></li>
</ul>

## News

<ul class="news-list" aria-label="News, newest first">
  <li><strong><time datetime="2026-09">2026.09</time></strong> — Started my Ph.D. at <strong>Fudan University</strong>.</li>
  <li><strong><time datetime="2026-08">2026.08</time></strong> — <strong>DEPPO</strong> was accepted to the <strong>EMNLP 2026 Main Conference</strong>.</li>
  <li><strong><time datetime="2026-06">2026.06</time></strong> — Graduated from <strong>Wuhan University</strong>, ranked <strong>1st out of 231</strong> students.</li>
  <li><strong><time datetime="2025-11">2025.11</time></strong> — Joined the Visual Understanding R&amp;D Center at <strong>TeleAI</strong>.</li>
  <li><strong><time datetime="2025-10">2025.10</time></strong> — Received the <strong>National Scholarship</strong>.</li>
  <li><strong><time datetime="2024-10">2024.10</time></strong> — Received the <strong>National Scholarship</strong>.</li>
  <li><strong><time datetime="2023-10">2023.10</time></strong> — Received the <strong>Lei Jun Computer Science Undergraduate Scholarship</strong>.</li>
</ul>

## Publications

{% include sections/publications.html %}

## Projects

{% include sections/projects.md %}

## CV

{% include sections/cv.md %}
