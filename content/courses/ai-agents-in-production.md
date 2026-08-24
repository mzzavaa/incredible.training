---
title: "AI Agents in Production"
description: "Take an agent system that works on your machine and make it something a team can deploy, evaluate, cost, and operate."
weight: 60
draft: false
course_code: "AGT-400"
level: "Advanced"
duration: "3 days"
formats: ["Three day intensive", "Cohort", "Private in-house"]
languages: ["English", "German"]
audience: "Teams that have a working prototype and now have to run it for real."
tools: ["AWS Bedrock", "MCP", "OpenTelemetry", "Terraform"]
track: "Building with AI"
prerequisites: "Building Agent Crews, or an agent system you have already built and want to ship."
---

**Purpose.** A large share of multi-agent pilots never survive contact with production. This is the
course about the gap between a demo that impresses and a system somebody has to be on call for.

**Contains.**
- The honest opening: why pilots die. Cost that only appears at volume, no evaluation, nobody owning
  the thing, and a failure mode nobody triggered before launch
- Evaluation before deployment: building a harness that catches regressions, cases derived from real
  failures, and why "it looked good in the demo" is not a test
- Deliberately breaking it in staging: run loops until the limit fires, feed oversized context to
  watch truncation, inject a wrong answer early in a chain and follow it downstream
- Cost engineering: measuring per task rather than estimating per month, model routing between a
  strong reasoning model and a cheaper utility model, caching, and scale-to-zero
- Observability: tracing every tool call, what to log, and what a useful alert looks like for a
  non-deterministic system
- Guardrails and human-in-the-loop: where a person must sign off, and how to design that without
  destroying the throughput that justified the system
- Deployment and reproducibility: infrastructure as code, environments, and rebuilding from scratch
- Operating it: ownership, runbooks, what changes when a model version moves under you
- Reference architecture slot, with the constraint stated: when not to use this shape
- Participants take a prototype through evaluation, cost analysis, and a deployment path

**Primary CTA.** Book a seat, or bring your own system and run it in-house.
**Links to.** /courses/building-agent-crews/, /for-teams/, /learning-paths/, https://incredible-consulting.com/ for delivery rather than enablement.
