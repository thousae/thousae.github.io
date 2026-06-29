---
layout: page
title: Research
permalink: /research/
---

## Research interests

I work on systems for serving LLM agents efficiently. My main interest is what happens after we move from single prompt-response inference to long-running agent workflows: agents call tools, update files, keep memory, revisit earlier tasks, and create intermediate state that may be useful again later.

This creates a serving problem. The system has to decide what to keep, what to reuse, and what to recompute. I am especially interested in memory and cache mechanisms for that setting.

Current areas I care about:

- LLM agent serving systems
- working memory and KV-cache reuse
- function-level computation reuse and cache grafting
- memory hierarchy for agent workloads
- consistency between stored memory and active context
- latency, memory footprint, and cost evaluation for agent serving

## Research direction

A recurring question in my work is: what is the right reusable unit in an agent workflow?

For normal LLM serving, the unit is often a request, a prompt prefix, or a KV-cache block. Agent workloads are messier. A useful unit might be a function call, a tool result, a memory object, a workflow fragment, or a partially reusable context span. Reusing the wrong thing can save time but introduce stale context. Recomputing everything is safer but expensive.

I study systems that make this tradeoff explicit. The goal is to reduce latency and memory cost while keeping the agent's active context consistent with its current memory and workspace state.

## Publications

### International conferences

1. **[Functional Cache Grafting: Robust and Rapid Code-Policy Synthesis for Embodied Agents](https://icml.cc/virtual/2026/poster/62313)**  
   **Saehun Chun**, Wonje Choi, Sera Choi, Sanghyun Ahn, and Honguk Woo*.  
   *International Conference on Machine Learning (ICML), 2026.*  
   FCGraft studies cache reuse at the function or workflow-fragment level for agentic workflows.  

2. **[Efficient Skill Grounding via Code Refactoring with Small Language Models](https://icml.cc/virtual/2026/poster/65138)**  
   Sera Choi, Wonje Choi, **Saehun Chun**, Daehee Lee, Chaeun Lee, Jooyoung Kim, and Honguk Woo*.  
   *International Conference on Machine Learning (ICML), 2026.*  
   This work studies efficient skill grounding by using small language models to refactor code.  

### Domestic conferences

1. **Undo Read Buffer: Preventing Buffer Pollution due to Undo Blocks in HTAP Workloads**  
   **Saehun Chun**, Jonghyeok Park, Sang-Won Lee*, and Young Ik Eom.  
   *Korea Computer Congress (KCC), 2024.*  
   This work studies buffer pollution caused by undo blocks in HTAP workloads and proposes an undo-read buffer mechanism to reduce that pollution.

2. **Analysis of Buffer Pollution Caused by Undo Pages in HTAP Workloads**  
   **Saehun Chun**, Bo-Hyun Lee, Kyong-Shik Lee, Sang-Won Lee*, and Young Ik Eom.  
   *Korean DataBase Conference (KDBC), 2023.*  
   This work analyzes how undo pages pollute the buffer pool under mixed transactional and analytical workloads.

