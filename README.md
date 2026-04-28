# Higgsfield MCP Bundle for OpenClaw

Claude-format bundle for Higgsfield's official remote MCP connector.

- Official landing page: <https://higgsfield.ai/mcp>
- MCP endpoint: `https://mcp.higgsfield.ai/mcp`
- No OpenClaw API keys required; authenticate through Higgsfield's connector flow.

## Install locally

Clone or download this repository, then install the bundle directory:

```bash
git clone https://github.com/efe-arv/openclaw-higgsfield-mcp-bundle.git
openclaw plugins install ./openclaw-higgsfield-mcp-bundle
openclaw plugins enable higgsfield
openclaw gateway restart
```

Requires an OpenClaw version with bundle MCP HTTP transport support.

## What it includes

- `.claude-plugin/plugin.json` Claude-format bundle manifest
- `.mcp.json` remote MCP server config
- `skills/higgsfield/SKILL.md` usage guidance for agents

## Security and cost notes

Higgsfield generations consume your Higgsfield credits. Confirm before bulk or expensive runs, and avoid pasting session tokens or account credentials into prompts or logs.
