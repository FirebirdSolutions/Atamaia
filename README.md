# Atamaia

**AI platform for identity, memory, and agent orchestration.**

Atamaia is a three-layer platform that gives AI agents persistent identity, long-term memory, and coordinated execution. Built for teams that need AI systems that remember, learn, and work together.

> *Atamaia* — from te reo Māori: *atamai* (intelligence, wisdom) + *maia* (brave, confident). Built in Aotearoa.

## What It Does

### Identity & Continuity
Persistent AI identities with cognitive state, emotional awareness, and session-to-session continuity. Agents aren't disposable — they build context over time.

### Memory Architecture
Hebbian memory with co-activation strengthening, typed links (temporal, causal, semantic, emotional, procedural), and hybrid search (full-text shortlist + vector ranking). Memories consolidate, strengthen, and decay naturally.

### Agent Orchestration
Multi-agent execution with task decomposition, dependency scheduling, budget management, and human-in-the-loop escalation. Agents spawn children, checkpoint progress, and recover from failures.

### Structured Hydration
Context assembled from parallel sources — identity, relationships, projects, memories, presence — injected on every interaction. Involuntary recall surfaces forgotten context when relevant.

## Architecture

```
Interaction Layer    MCP Server | REST API | Agent Adapter | CLI
Core Services        Memory | Identity | Communication | Projects | AI Routing
Autonomic Layer      Wingman | Consolidation | Guardian
Database             PostgreSQL + pgvector
```

## Key Design Principles

- **API-first** — REST is source of truth, all other interfaces wrap it
- **Multi-tenant** — isolated tenants from day one
- **Soft delete only** — nothing is ever truly lost
- **Feedback loops** — agent run ratings feed back into future confidence
- **Diagnose before retry** — four failure modes detected, each handled differently
- **Concrete loop detection** — duplicate reads and repeated tool calls, not abstract progress metrics

## Tech Stack

- .NET 10 / ASP.NET Core
- PostgreSQL + pgvector
- React 19 / Vite / Tailwind / shadcn/ui
- MCP (Model Context Protocol) server
- JWT authentication with refresh token rotation

## Status

Active development. Not yet open source — watching this space.

## Built By

[Firebird Solutions](https://firebird.nz) — Rich & Ash, Aotearoa New Zealand.

## Links

- Website: [atamaia.ai](https://atamaia.ai)
- Developer docs: [atamaia.dev](https://atamaia.dev)
