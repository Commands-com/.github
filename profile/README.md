<div align="center">

# Commands.com

**Local AI rooms where independent models converge.**

[![Beta](https://img.shields.io/badge/Beta-Sign%20Up-2563EB.svg)](https://commands.com/beta/)
[![Gateway](https://img.shields.io/badge/Gateway-OSS-0B0D0E.svg)](https://github.com/Commands-com/gateway)
[![Room Plugins](https://img.shields.io/badge/Rooms-Plugins-14B8A6.svg)](https://github.com/Commands-com/room-plugins)
[![E2EE](https://img.shields.io/badge/Relay-E2EE-8B5CF6.svg)](https://github.com/Commands-com/gateway)

Orchestrated rooms running on your machine. Multiple AI models explore, build, and audit independently — converging on solutions proven by real metrics, not model confidence.

</div>

---

## Why Convergence

One model playing five roles still has one set of blind spots. Giving it five personas doesn't give you five perspectives — it gives you one perspective in five costumes.

Commands.com runs **rooms** — orchestrated workspaces where independent models with different training data, architectures, and tooling converge on a shared objective through a structured pipeline.

> The most reliable AI is not one model. It's independent models that converge.
>
> — [The Great Convergence](https://thegreatconvergence.com)

## The Pipeline

Every room follows a convergence cycle:

```
Fan Out          →   Synthesize       →    Build            →    Audit
Multiple             Merge, dedup,         Implement top         Independent
explorers            rank by               candidates,           validation for
discover             consensus             benchmark with        production risk
independently                              real metrics
```

```
Explored: 12  →  Synthesized: 5  →  Built: 3  →  Converged: 1
```

## Agent Roles

| Role | What it does | Why a separate model |
|---|---|---|
| **Explorer** | Casts the widest net across candidates | Different search corpora and training data maximize diversity of discovery |
| **Builder** | Implements with precision, benchmarks empirically | The strongest agentic coder, informed by consensus from explorers |
| **Auditor** | Validates for production safety and correctness | Independent scrutiny catches what the builder's biases miss |

## Platform

| Repo | What it does | Stack |
|---|---|---|
| [gateway](https://github.com/Commands-com/gateway) | Self-hosted encrypted relay, OAuth/OIDC, device routing, shares, webhook tunnel, admin console | Go |
| [agent-workspace](https://commands.com/beta/) | Local runtime, rooms engine, desktop app, CLI, audit logging, remote chat, MCP passthrough | TS / Electron / Node |
| [room-plugins](https://github.com/Commands-com/room-plugins) | Room orchestrators for domain-specific convergence — SQL optimization, FFT autotuning, and more | JS plugins |
| [interface-plugins](https://github.com/Commands-com/interface-plugins) | External interface providers for webhook and Slack-style integrations | JS plugins |
| [agent-plugins](https://github.com/Commands-com/agent-plugins) | Provider plugins that make model diversity real instead of cosmetic | JS plugins |

## Rooms in Practice

**Postgres Query Optimizer** — Explorers independently discover index strategies and query rewrites. The builder implements each candidate against a real Postgres instance, measuring actual execution time. The auditor validates for production safety.

**FFT Autotune** — Explorers search for SIMD vectorization strategies across Apple Silicon architectures. The builder compiles and benchmarks each kernel variant. The auditor validates numerical accuracy. Convergence means the fastest correct implementation wins.

## Security

- End-to-end encrypted relay (AES-256-GCM) — we can't read your data, even if we wanted to
- Rooms, agents, code, and data stay on your machine
- Self-hosted gateway option for teams that want infrastructure ownership
- Zero-knowledge architecture — by design, not by policy

## Get Started

**[Sign up for the beta](https://commands.com/beta/)** to get early access to the desktop app and start running rooms locally.

```bash
# Self-host the relay
git clone https://github.com/Commands-com/gateway.git

# Extend with plugins
git clone https://github.com/Commands-com/room-plugins.git
git clone https://github.com/Commands-com/agent-plugins.git
git clone https://github.com/Commands-com/interface-plugins.git
```

<div align="center">

[commands.com](https://commands.com) · [The Great Convergence](https://thegreatconvergence.com) · [Discord](https://discord.gg/snk8BEHfRd)

</div>
