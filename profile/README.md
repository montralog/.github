<p align="center"><img src="https://raw.githubusercontent.com/montralog/montralog/main/docs/assets/montralog-avatar.png" width="96" alt="Montralog"></p>

# Montralog

**Monitoring · Tracing · Logging · Tracking**

Open-source, self-hosted observability for understanding infrastructure and applications. Bring logs, traces, recurring patterns, Prometheus metrics, dashboards and alerts into one workspace.

### Get started with 0.5.1

- [Stable release and verified downloads](https://github.com/montralog/montralog/releases/tag/v0.5.1)
- [Docker quickstart](https://github.com/montralog/montralog#quickstart) · [Public container package](https://github.com/montralog/montralog/pkgs/container/montralog)
- [Helm deployment](https://github.com/montralog/montralog/blob/main/deploy/helm/montralog/README.md) · [Artifact Hub](https://artifacthub.io/packages/helm/montralog/montralog)
- [Organization rollout guide](https://github.com/montralog/montralog/blob/main/docs/ORGANIZATION_ROLLOUT.md)
- [Documentation](https://github.com/montralog/montralog/tree/main/docs) · [Contribute or report a bug](https://github.com/montralog/montralog/blob/main/CONTRIBUTING.md)

```sh
docker pull ghcr.io/montralog/montralog:0.5.1
```

Use the deployment guides to configure persistent storage, credentials and the required encryption key before starting an instance. The published image supports Linux/amd64.

### Built for self-hosting

Docker Compose and Helm deployments, SQLite for a single gateway, optional PostgreSQL for multiple gateways, and Prometheus for metrics. Create graphs, stats, tables and timelines; manage scoped API tokens, notification rules, teams and groups.

Company sign-in configuration supports Microsoft Entra ID, Google Workspace and Okta. Provider registration and live tenant verification are required. Vendor audit polling and directory synchronization are not implemented.

### Release verification

0.5.1 passed 151 Python tests on each of Python 3.11 and 3.13, three frontend tests, four Chromium acceptance cases, Docker checks and Kubernetes deployment checks. The published image's scan reported zero HIGH/CRITICAL findings. Checksums, security reports, dependency inventory and browser results accompany the release; the image includes GitHub build provenance.

Read the [verification evidence](https://github.com/montralog/montralog/blob/main/docs/SECURITY_VERIFICATION-0.5.1.md), [support scope](https://github.com/montralog/montralog/blob/main/docs/SUPPORT.md) and [rollout requirements](https://github.com/montralog/montralog/blob/main/docs/ORGANIZATION_ROLLOUT.md). Production use requires acceptance in your own environment, including networking/TLS, tenant integrations, capacity and recovery. A passing scan is a snapshot, not an independent audit.

First-party code is [Apache-2.0](https://github.com/montralog/montralog/blob/main/LICENSE). Contributions and reproducible feedback are welcome. Please [report security issues privately](https://github.com/montralog/montralog/security/advisories/new).
