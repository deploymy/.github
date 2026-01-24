<a href="https://deploystack.io">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="/profile/deploystack-github-banner-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="/profile/deploystack-github-banner-white.png">
    <img alt="DeployStack" src="/profile/deploystack-github-banner-white.png">
  </picture>
</a>

**Open source MCP hosting platform** — deploy MCP servers from GitHub to HTTP endpoints in 30 seconds.

## The Problem

Most MCP servers are **stdio-only**. But workflow automation platforms need **HTTP endpoints**:

| Platform | The Problem |
|----------|-------------|
| **n8n** | MCP Client node requires HTTP URLs |
| **Dify** | HTTP/SSE only (v1.6+) |
| **Voiceflow** | "Local MCP NOT supported" |
| **Langflow** | HTTP/SSE for production workflows |

Current workarounds are painful:
- `mcp-remote` requires local Node.js setup
- Docker containers need DevOps expertise
- DIY hosting takes hours

**And for teams**, credentials scatter across Slack DMs and `.env` files. No visibility into who uses what. Onboarding takes hours.

## The Solution

### Deploy from GitHub

1. Connect your GitHub account
2. Select a repository with an MCP server
3. Get an HTTP endpoint that works immediately

Auto-deploys when you push. Like Vercel, but for MCP servers.

### Or Use the Curated Catalog

Browse 1,000+ pre-configured MCP servers. One-click install, ready in seconds.

## Key Features

| Feature | What It Does |
|---------|--------------|
| **Deploy from GitHub** | Any MCP repo → HTTP endpoint in 30 seconds |
| **98% Token Reduction** | Hierarchical router: 2 meta-tools instead of 150 tools |
| **Credential Vault** | Encrypted storage, automatic injection at runtime |
| **Team Management** | RBAC, audit logging, team isolation |
| **Works Everywhere** | n8n, Dify, Voiceflow, Langflow, Claude Code, Cursor |

### How Token Reduction Works

Traditional setup: 10 servers × 15 tools = 150 tools = **75,000 tokens** consumed before you start.

DeployStack's hierarchical router exposes 2 meta-tools:
- `discover_mcp_tools` — search for tools by keyword
- `execute_mcp_tool` — run the tool you need

Result: **1,372 tokens** instead of 75,000. Scale to 100+ MCP servers without performance degradation.

## Repositories

**[deploystack](https://github.com/deploystackio/deploystack)** — Main platform: backend API, frontend dashboard, satellite service

**[documentation](https://github.com/deploystackio/documentation)** — Deployment guides and API docs

## Getting Started

**Try it free:** [cloud.deploystack.io](https://cloud.deploystack.io)

**Self-host:** [docs.deploystack.io/self-hosted/quick-start](https://docs.deploystack.io/self-hosted/quick-start)

**Documentation:** [docs.deploystack.io](https://docs.deploystack.io)

## Open Source

DeployStack is licensed under **AGPL-3.0**. Self-host on your infrastructure or use our managed cloud.

## Contributing

We welcome contributions in:

- MCP server integrations
- Satellite infrastructure
- Documentation
- Enterprise features

Check [CONTRIBUTING.md](https://github.com/deploystackio/deploystack/blob/main/CONTRIBUTING.md) for details.

---

**Questions?** Join our [Discord](https://discord.gg/42Ce3S7b3b) or check the [docs](https://docs.deploystack.io).
