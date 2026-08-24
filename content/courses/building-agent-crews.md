---
title: "Building Agent Crews"
description: "Move from one agent to several working together: orchestration patterns, handoffs, retrieval, and the failure modes that appear the moment you add a second agent."
weight: 50
draft: false
course_code: "BAC-300"
level: "Advanced"
duration: "2 days"
formats: ["Two day intensive", "Cohort", "Private in-house"]
languages: ["English", "German"]
audience: "Engineers and architects who have built something with one agent and now need several to cooperate."
tools: ["Kiro crew", "Hermes agents", "Claude Code", "MCP"]
track: "Building with AI"
prerequisites: "Coding with Agents, or equivalent hands-on experience with a coding agent."
---

**Purpose.** One agent doing one task is a solved problem. The difficulty starts at two. This course
is about the patterns that hold up and the ones that quietly do not.

**Contains.**
- When a crew is the right answer and when a single agent with better tools is simply cheaper. Most
  multi-agent designs should have stayed single-agent
- The orchestration patterns worth knowing, with the tradeoff for each: supervisor, pipeline,
  fan-out, debate, swarm. Supervisor first, because it has the widest framework support and the
  best-understood failure mode
- Handoffs, where most crews break: what context travels between agents, what gets dropped, and why
  disparate tool sets between agents make it worse
- Tools and MCP: giving agents capability deliberately rather than handing them everything
- Retrieval as a component: when a crew needs grounding in your own material, how to wire it, and
  how to keep answers traceable to a source
- Hands-on with crew-style orchestration, including Kiro crew and Hermes agents, kept at the level
  of the pattern rather than the vendor, since the products move faster than the concepts
- The failure modes, triggered deliberately in a lab: infinite loops, context truncation, one
  agent's hallucination propagating down the chain, over-delegation by the supervisor
- Cost, stated plainly. Orchestration multiplies calls. A design that costs cents in testing can
  cost a great deal in production, and the arithmetic belongs in the design review
- Each participant leaves with a working crew and a written account of how they broke it

**Primary CTA.** Book a seat, or run it in-house on a system you are already building.
**Links to.** /courses/coding-with-agents/, /courses/ai-agents-in-production/, /learning-paths/, /schedule/.
