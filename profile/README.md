<div align="center">

# Commands.com

**Local-first AI workspaces for independent models that converge.**

[![Gateway](https://img.shields.io/badge/Gateway-OSS-0B0D0E.svg)](https://github.com/Commands-com/gateway)
[![Agent Workspace](https://img.shields.io/badge/Agent%20Workspace-Desktop%20%26%20CLI-43853d.svg)](https://github.com/Commands-com/agent-workspace)
[![Plugins](https://img.shields.io/badge/Plugins-Agents%20%7C%20Rooms%20%7C%20Interfaces-2563EB.svg)](https://github.com/Commands-com/room-plugins)
[![Relay Security](https://img.shields.io/badge/Relay-E2EE-8B5CF6.svg)](https://github.com/Commands-com/gateway)

Build AI workflows that run where your code lives, connect through an encrypted gateway, and stay extensible with plugins and rooms instead of forks.

```text
Local Agent Workspace + Plugins  <── E2EE / Webhooks / Shares ──>  OSS Gateway  <──> Browser / Desktop Clients
```

</div>

---

## Platform

Commands.com is a local-first platform for running AI near your code, sharing access through a self-hosted relay, and composing provider, room, and interface plugins into structured multi-model systems.

| Repo | What it does | Stack |
|---|---|---|
| [gateway](https://github.com/Commands-com/gateway) | Self-hosted encrypted relay, OAuth/OIDC, device routing, shares, webhook tunnel, admin console | Go |
| [agent-workspace](https://github.com/Commands-com/agent-workspace) | Local runtime, CLI, desktop app, audit logging, remote chat, MCP passthrough | TypeScript, Electron, Node.js |
| [room-plugins](https://github.com/Commands-com/room-plugins) | External room orchestrators for multi-step and multi-agent workflows | JavaScript plugins |
| [interface-plugins](https://github.com/Commands-com/interface-plugins) | External interface providers for webhook and Slack-style integrations | JavaScript plugins |
| [agent-plugins](https://github.com/Commands-com/agent-plugins) | External provider plugins for model and runtime integrations | JavaScript plugins |

## Core Ideas

| | |
|---|---|
| **Local-first execution** | Agents run near your code, files, MCP servers, and internal systems |
| **Independent model convergence** | Reliability improves when genuinely different models explore, build, and audit independently, then agree |
| **Room-based specialization** | Rooms make workflows explicit so roles like exploration, synthesis, building, and auditing are reusable instead of improvised |
| **Encrypted relay** | Gateway routes sessions and events without becoming the place your work lives |
| **Bring your own infrastructure** | The relay is OSS and self-hostable |
| **Plugin-first extension model** | Agents, rooms, and interfaces can be extended in separate repos |
| **Workspace + control plane** | The local workspace and relay stay cleanly separated |

## How The Pieces Fit

1. Start the [agent-workspace](https://github.com/Commands-com/agent-workspace) on your machine.
2. Connect it to the [gateway](https://github.com/Commands-com/gateway) for auth, routing, session sharing, and webhook ingress.
3. Add custom providers from [agent-plugins](https://github.com/Commands-com/agent-plugins) to bring different model families and runtimes into the same workspace.
4. Add orchestrators from [room-plugins](https://github.com/Commands-com/room-plugins) to fan out work, synthesize findings, and route specialized roles.
5. Add webhook or chat-style ingress from [interface-plugins](https://github.com/Commands-com/interface-plugins).

## What We Optimize For

- Your code stays local.
- Different models can stay genuinely different instead of pretending to be a team through prompt personas.
- Rooms and plugins make specialization explicit and reusable.
- The gateway is a relay and control plane, not your runtime.
- Teams can share agents and interfaces without collapsing everything into one monolith.

## Start Here

```bash
# Self-host the relay
git clone https://github.com/Commands-com/gateway.git

# Run the local workspace
git clone https://github.com/Commands-com/agent-workspace.git

# Extend the platform
git clone https://github.com/Commands-com/room-plugins.git
git clone https://github.com/Commands-com/interface-plugins.git
git clone https://github.com/Commands-com/agent-plugins.git
```

## Repo Focus

- **Gateway**: self-hosted encrypted relay with console, OAuth, device routing, shares, and webhook tunneling.
- **Agent Workspace**: local CLI and desktop app for running agents, chatting remotely, and managing multi-model workflows near your code.
- **Room Plugins**: external orchestrator types for structured workflows, specialization, and multi-agent collaboration.
- **Interface Plugins**: ingress adapters for external systems and webhook-style integrations.
- **Agent Plugins**: provider and runtime plugins that make model diversity real instead of cosmetic.

## Security Model

- End-to-end encrypted relay sessions between clients and local agents.
- Local execution for code access, tools, and MCP servers.
- Clear split between runtime state and relay/control-plane concerns.
- Self-hosted gateway option for teams that want infrastructure ownership.

## Build With Us

If you want to self-host, start with [gateway](https://github.com/Commands-com/gateway). If you want to run agents locally, start with [agent-workspace](https://github.com/Commands-com/agent-workspace). If you want to build specialized, multi-model workflows, start with [room-plugins](https://github.com/Commands-com/room-plugins) and [agent-plugins](https://github.com/Commands-com/agent-plugins). If you want external ingress, add [interface-plugins](https://github.com/Commands-com/interface-plugins).
