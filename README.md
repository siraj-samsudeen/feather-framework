# Feather Framework

An ecosystem for building apps and data platforms faster with AI agents.

Feather is a family of client-facing products, frameworks, and developer packages, organized in three tiers: **Products** you deploy for clients, **Frameworks** you build on, and **Dev packages** that support the building.

## Products

Client-facing products, deployed per client for retail and business customers. Each instance is displayed as "{Client} {Noun}" — e.g. a client named Acme runs "Acme Answers".

| Product | What it does |
|---------|--------------|
| **Feather Answers** | Governed question-and-answer over your data warehouse, delivered as a connector for AI chat. Business users ask questions in plain language and get answers from curated warehouse tables — with the house rules (metric definitions, filters, access boundaries) enforced. |
| **Feather Reports** | Pre-rendered HTML dashboards and reports, served fast and simple from a lightweight report server — by default at `reports.<client-domain>`. |

Product implementations live in per-client engagements; this page describes capability only.

## Frameworks

The mid-tier: things developers build on.

| Package | Description | Status |
|---------|-------------|--------|
| [featherbase](https://github.com/siraj-samsudeen/featherbase) | Metadata-driven app platform in TypeScript — Frappe's core ideas on Convex + React, with Glide-style workflows and AI-agent-first authoring. | In Progress |
| [feather-flow](https://github.com/siraj-samsudeen/feather-flow) | Lightweight, config-driven data pipelines in Python — a full extract-transform-publish stack in one small package. | Active |
| [feather-skills](https://github.com/siraj-samsudeen/feather-skills) | Agent workflow skills for Claude Code — brainstorm → spec → execute, gated at every step. Stack-agnostic. | Active |

## Dev packages

Low-level packages and templates that support building with Feather.

| Package | Description | Status |
|---------|-------------|--------|
| [feather-testing-core](https://github.com/siraj-samsudeen/feather-testing-core) | Phoenix Test-inspired fluent testing DSL for Playwright and RTL. Stack-agnostic. | Active |
| [feather-testing-convex](https://github.com/siraj-samsudeen/feather-testing-convex) | Phoenix/Wallaby-inspired integration testing for React + Convex. | Active |
| [feather-starter-convex](https://github.com/siraj-samsudeen/feather-starter-convex) | Production-ready SaaS starter for React + Convex + Vite. | In Progress |
| [feather-example-app](https://github.com/siraj-samsudeen/feather-example-app) | Reference app showcasing the Feather ecosystem (Convex + Auth + testing DSL). | Active |
| [feather-gsd](https://github.com/siraj-samsudeen/feather-gsd) | Meta-prompting, context engineering and spec-driven development system for Claude Code and OpenCode. | Active |

## Naming Convention

Two registers, one per audience:

- **Builder tools** (frameworks and dev packages): `feather-{function}`, lowercase — e.g. `feather-skills`. Stack-specific variants add the stack: `feather-{function}-{stack}` — e.g. `feather-testing-convex`.
- **Products** (client-facing): **Feather {Noun}**, Title case — e.g. Feather Answers. Client instances are displayed as "{Client} {Noun}".

### Renames (2026-07-17)

- `feather-etl` → **feather-flow** (data pipelines). Old URLs redirect; the PyPI package is still published as `feather-etl` for now.
- The former `feather-flow` (agent workflows) → **feather-skills**. The npm package is still published as `feather-flow` for now.

## Philosophy

- **Convention over configuration** — Sensible defaults, override when needed
- **AI-first development** — Skills and patterns designed for agent-assisted workflows
- **Test-driven** — Every package ships with testing support built in
- **Inspired by the best** — Phoenix, Rails, Wallaby, Frappe — adapted for modern stacks

## Roadmap

Future packages under consideration:

- `feather-starter-supabase` — Starter for Supabase stack
- `feather-starter-instantdb` — Starter for InstantDB stack
