---
layout: page
title: About
permalink: /about/
---

I am a researcher working on efficient serving for LLM agents. My current work focuses on memory and cache reuse in long-running agentic workflows, where agents repeatedly plan, call tools, update workspace state, and return to related contexts over time.

A central question in my research is how serving systems should represent and reuse intermediate state. Instead of treating every agent request as independent, I study reusable units such as function-level computation, working memory objects, tool results, and KV-cache spans. The goal is to reduce latency and memory cost while preserving correctness when the agent's context changes.

I am especially interested in the boundary between LLM serving systems and agent workloads: how new interaction patterns create new bottlenecks, and how memory/cache systems should adapt to them.

## Contact

For research discussions or collaboration, please use the links on the home page or contact me through my listed academic/profile channels.
