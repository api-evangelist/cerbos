---
title: "Agent Skill for Writing Authorization Policies in Claude Code"
url: "https://www.cerbos.dev/blog/agent-skill-for-writing-authorization-policies-in-claude-code"
date: "2026-06-02"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/blog"
---
The Cerbos policy skill for Claude Code integrates authorization policy generation directly into the developer terminal, with generated YAML and CEL policies depositing into the repository, compiling against the actual Cerbos binary, and validating through tests before commit. This addresses the complexity of managing multi-resource authorization policies with derived roles, attribute conditions, and multi-tenant configurations that consume development time on repetitive tasks. The guide covers skill installation, typical Claude Code workflows, how validation works against the real compiler, and which decisions require human judgment.
