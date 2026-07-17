# Feather Framework

An ecosystem for building apps faster with AI agents.

Feather is a collection of packages, starter templates, and agent skills designed to make full-stack development with AI assistants productive and enjoyable.

## Ecosystem

| Package | Description | Status |
|---------|-------------|--------|
| [feather-skills](https://github.com/siraj-samsudeen/feather-skills) | Skills and workflows for AI coding agents. Stack-agnostic. | Active |
| [feather-starter-convex](https://github.com/siraj-samsudeen/feather-starter-convex) | Starter template for React + Convex + Vite. | In Progress |
| [feather-testing-core](https://github.com/siraj-samsudeen/feather-testing-core) | Phoenix Test-inspired fluent testing DSL for Playwright and RTL. Stack-agnostic. | Active |
| [feather-testing-convex](https://github.com/siraj-samsudeen/feather-testing-convex) | Phoenix/Wallaby-inspired integration testing for React + Convex. | Active |
| [feather-example-app](https://github.com/siraj-samsudeen/feather-example-app) | Reference app showcasing the Feather ecosystem (Convex + Auth + testing DSL). | Active |

## Naming Convention

- **`feather-{function}`** — Stack-agnostic packages (e.g., `feather-skills`)
- **`feather-{function}-{stack}`** — Stack-specific packages (e.g., `feather-testing-convex`, `feather-starter-convex`)

## Philosophy

- **Convention over configuration** — Sensible defaults, override when needed
- **AI-first development** — Skills and patterns designed for agent-assisted workflows
- **Test-driven** — Every package ships with testing support built in
- **Inspired by the best** — Phoenix, Rails, Wallaby — adapted for the JS/TS ecosystem

## Roadmap

Future packages under consideration:

- `feather-analytics` — Analytics integration
- `feather-flow` (renamed from `feather-etl`, 2026-07-17) — Data pipeline utilities
- `feather-starter-supabase` — Starter for Supabase stack
- `feather-starter-instantdb` — Starter for InstantDB stack
