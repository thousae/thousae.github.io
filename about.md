---
layout: page
title: About
permalink: /about/
---

I am a researcher working on efficient serving for LLM agents. My current work focuses on memory and cache reuse in long-running agentic workflows, where agents repeatedly plan, call tools, update workspace state, and return to related contexts over time.

A central question in my research is how serving systems should represent and reuse intermediate state. Instead of treating every agent request as independent, I study reusable units such as function-level computation, working memory objects, tool results, and KV-cache spans. The goal is to reduce latency and memory cost while preserving correctness when the agent's context changes.

I am especially interested in the boundary between LLM serving systems and agent workloads: how new interaction patterns create new bottlenecks, and how memory/cache systems should adapt to them.

## Education

- **Integrated M.S./Ph.D. Program in Software**, Sungkyunkwan University, 2025–Present. Advisor: Honguk Woo.
- **B.S. in Software**, Sungkyunkwan University, 2019–2024.

## Research experience

- **Graduate Researcher**, CSI Lab, Sungkyunkwan University, 2024–Present. Memory systems and cache reuse for LLM agents.
- **Undergraduate Research Assistant**, VLDB Lab, Sungkyunkwan University, 2023–2024. Memory management and buffer-pool behavior in HTAP workloads.

## Teaching

- **Hands-on Training Instructor** · GenAI PowerUser Program Level 4 (Multi Agent framework), Samsung Electronics University · 2026–Present.
- **Hands-on Training Instructor** · Artificial Intelligence Project, Sungkyunkwan University · Fall 2026.
- **Teaching Assistant** · System Programming, Sungkyunkwan University · Spring 2026.
- **Teaching Assistant** · Mobile Application Programming, Sungkyunkwan University · Spring 2025.

## Awards

Graduate Research Fellowship, National Research Foundation of Korea, 2025–2026.

## Contact

For research discussions or collaboration: [{{ site.author.email }}](mailto:{{ site.author.email }}).
