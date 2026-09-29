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

{% include publications.html detailed=true %}
