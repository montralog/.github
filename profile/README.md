<p align="center"><img src="https://raw.githubusercontent.com/montralog/montralog/main/docs/assets/montralog-avatar.png" width="96" alt="Montralog"></p>

# Montralog

**Monitoring · Tracing · Logging · Tracking**

Open-source observability for infrastructure and applications. Explore logs, traces, recurring patterns, Prometheus metrics, dashboards and alerts in one workspace.

### Start with Docker

**Stable release: 0.8.0.** Linux/amd64. Docker Engine/Desktop with Compose v2 is the installation path; host Python, Helm and Kubernetes are not required.

```sh
docker pull ghcr.io/montralog/montralog:0.8.0
```

- [Install with Docker](https://github.com/montralog/montralog/blob/main/docs/CONTAINERS.md)
- [Release downloads and checksums](https://github.com/montralog/montralog/releases/tag/v0.8.0) · [Public container package](https://github.com/montralog/montralog/pkgs/container/montralog)
- [Published security, bootstrap and load/recovery reports](https://github.com/montralog/montralog/blob/main/docs/reports/README.md)
- [Customer isolation](https://github.com/montralog/montralog/blob/main/docs/TENANCY.md) · [Production acceptance matrix](https://github.com/montralog/montralog/blob/main/docs/PRODUCTION.md)
- [Documentation](https://github.com/montralog/montralog/tree/main/docs) · [Contributing](https://github.com/montralog/montralog/blob/main/CONTRIBUTING.md)

### Customer hosting and security

Use separate Docker projects, databases, keys, tokens, networks and queues per customer. Database transactions and browser cookies are bound to customer identity. Shared-gateway/database SaaS hosting is disabled. Teams and groups manage membership within a customer.

Saved credentials require HTTPS. Outbound transport rejects redirects and unapproved private/metadata destinations, pins validated DNS addresses and preserves TLS certificate verification. Encrypted credential migration and backup/key recovery have regression coverage.

Release checks cover Python 3.11/3.13, browser behavior, Docker and retained chart compatibility, dependency/static/image scans, private bootstrap and synthetic ingestion/recovery. Public reports retain all severities and static warnings. The exact scanned release image is tested before publication and includes build provenance.

### Read-only agentic investigations

Ask AI from a dashboard panel or investigate an alert with its saved runbook. Capture log, trace and change evidence with record references. The agent can inspect approved metrics within three model calls, with literal excerpts, missing evidence and a read-only trace. Optional local Ollama Qwen3 4B analysis uses durable jobs and budgets; hosted adapters require explicit sharing approval. Results remain unverified hypotheses. Approved runbooks currently perform read-only source checks. [AI setup and limits](https://github.com/montralog/montralog/blob/main/docs/AI-INVESTIGATIONS.md).

### Operating scope

Validate customer TLS, egress, backups, actual SSO/Slack destinations, sustained workload capacity and host/disk failure before relying on the deployment. Short synthetic measurements are not a capacity guarantee or independent audit. Host administrators remain trusted; whole-stack HA and shared-database SaaS have not been established.

Company sign-in configuration supports Microsoft Entra ID, Google Workspace and Okta; live provider registration is required. Vendor audit polling and directory synchronization are not implemented. Historical Helm artifacts remain available for existing deployments.

First-party code is [Apache-2.0](https://github.com/montralog/montralog/blob/main/LICENSE). Please [report security issues privately](https://github.com/montralog/montralog/security/advisories/new).
