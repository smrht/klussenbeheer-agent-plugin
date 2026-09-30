# Klussenbeheer agent plugin

Find jobs and customers, view your schedule, and add job notes using your existing Klussenbeheer account. Choose your company before each action. Changes require your confirmation and follow your existing account permissions. Technicians only access their assigned jobs. This plugin does not sell subscriptions or process payments.

## Connect

Use the public MCP endpoint `https://samdesk.nl/mcp` in a client supporting Streamable HTTP and OAuth. Sign in to your existing account and review the requested permissions. No API key belongs in this repository.

The root `plugin.json` and `mcp.json` support Agent Plugins clients. The compatibility manifests support Claude Code, Grok Build and Codex. The packaged skill describes when to use each tool and how to handle permissions and confirmations.

## Data and permissions

The connection sends tool arguments to the service at `https://samdesk.nl/mcp` and returns account-scoped records to your chosen assistant. Disconnecting the OAuth connection revokes future access. Treat returned customer or backlink records as private. No local telemetry or shell hooks are bundled.

[Product](https://samdesk.nl/plugin/) · [Privacy](https://samdesk.nl/plugin/privacy/) · [Terms](https://samdesk.nl/nl/terms-of-service/) · [Support](https://samdesk.nl/nl/contact/)

## Source and license

Maintained by Samautomation, the operator of this service. This repository contains only the public plugin package; the hosted application and account data are separate. The package is MIT-licensed; the hosted service uses its own terms.
