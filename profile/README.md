# Pipes.bot

**Talk to your AI agent on WhatsApp -- without getting banned.**

Pipes.bot is a managed bridge that connects self-hosted AI agents to Meta's official WhatsApp Cloud API. No exposed infrastructure, no unofficial libraries, no account bans.

## Examples

The fastest way to start is to copy a working example from [pipes-bot-examples](https://github.com/pipes-bot/pipes-bot-examples). Each folder is standalone, with its own dependencies and README:

```bash
npx degit pipes-bot/pipes-bot-examples/<folder> my-app
```

### Starters

A single file that receives WhatsApp messages and replies to them.

| Example | Stack | Description |
|---------|-------|-------------|
| [with-hono-bun](https://github.com/pipes-bot/pipes-bot-examples/tree/main/with-hono-bun) | Hono, Bun, TypeScript | Webhook receiver in a single Hono file on Bun |
| [with-nextjs-route-handler](https://github.com/pipes-bot/pipes-bot-examples/tree/main/with-nextjs-route-handler) | Next.js, TypeScript, Vercel | Webhook receiver in a single Next.js route handler, ready for Vercel |
| [with-fastapi](https://github.com/pipes-bot/pipes-bot-examples/tree/main/with-fastapi) | FastAPI, Python | Webhook receiver in a single FastAPI file |
| [with-websocket-node](https://github.com/pipes-bot/pipes-bot-examples/tree/main/with-websocket-node) | Node.js, TypeScript, ws | Receives messages over a WebSocket connection, no public URL needed |

### Apps

Full apps with sign-in, Embedded Signup and WhatsApp coexistence.

| Example | Stack | Description |
|---------|-------|-------------|
| [ai-handoff](https://github.com/pipes-bot/pipes-bot-examples/tree/main/ai-handoff) | TanStack Router, Convex, OpenRouter | An AI agent answers customers from your instructions and FAQ, and steps aside when your team replies from the phone |
| [mini-crm](https://github.com/pipes-bot/pipes-bot-examples/tree/main/mini-crm) | TanStack Router, Convex, MCP | A WhatsApp CRM with a pipeline, an inbox and an MCP server so Claude can read contacts and draft replies |
| [conversation-analyzer](https://github.com/pipes-bot/pipes-bot-examples/tree/main/conversation-analyzer) | TanStack Router, Convex, OpenRouter | Captures replies sent from the phone and scores each conversation on response time and your support methodology |

No phone? The examples repo ships a mock API and a webhook simulator so you can test a starter locally. See [Testing without a phone](https://github.com/pipes-bot/pipes-bot-examples#testing-without-a-phone).

## Why Pipes.bot

- Official WhatsApp Cloud API -- 99.9% delivery rate, <500ms median latency
- Outbound-only connections -- your agents stay private behind your firewall
- Message queue with offline delivery -- never miss a message
- Works with OpenClaw, webhooks, n8n, Make, Zapier, and custom apps
- Up and running in ~5 minutes

## Get Started

Create your account at [pipes.bot](https://pipes.bot) and read the docs at [docs.pipes.bot](https://docs.pipes.bot).

## Repositories

| Repo | Description |
|------|-------------|
| [pipes-bot-examples](https://github.com/pipes-bot/pipes-bot-examples) | Starters and full apps built on the Pipes.bot WhatsApp API |
| [pipes-bot-byon-demo](https://github.com/pipes-bot/pipes-bot-byon-demo) | Demo app for Bring Your Own Number (BYON) with Embedded Signup |
| [openclaw-whatsapp-api-channel](https://github.com/pipes-bot/openclaw-whatsapp-api-channel) | OpenClaw plugin for the Pipes.bot WhatsApp API channel |
| [claude-plugins](https://github.com/pipes-bot/claude-plugins) | Claude plugins for Pipes.bot integrations |
