---
layout: home
title: Home
---

## About

I work on memory and cache systems for efficient LLM agent serving. My research studies how long-running agentic workflows can reuse computation, working memory, and KV-cache state across repeated or evolving tasks without losing consistency.

## Current Focus

- **Agentic Memory Serving:** serving systems for LLM agents whose state grows across tool calls, files, plans, and conversations.

## Research Direction

Modern LLM agents do more than answer one prompt. They plan, call tools, edit files, observe state changes, and return to related tasks later. That shift breaks the usual assumption that each request can be served independently.

My work asks what should be reused across these workflows, at what granularity, and how serving systems can trade off latency, memory footprint, cost, and correctness. The core theme is simple: make agent serving faster and cheaper by reusing the right computation and memory state, while avoiding stale or inconsistent context.

