# Comettrace

**Open-source OpenTelemetry trace explorer, self-hostable or in the cloud.**

![Rust](https://img.shields.io/badge/Rust-stable-orange?logo=rust)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-OTLP-blueviolet?logo=opentelemetry)
![ClickHouse](https://img.shields.io/badge/ClickHouse-storage-yellow?logo=clickhouse)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-control%20plane-336791?logo=postgresql)
![License](https://img.shields.io/badge/license-AGPL--3.0%20%2F%20commercial-blue)

Comettrace receives your traces over OTLP and lets you explore them: every request, every service, every error, in one interface. The same code runs on your own infrastructure or in our cloud.

## Why Comettrace

- **Open source**: the core is public. Read it, change it, run it yourself.
- **OpenTelemetry native**: no proprietary SDK. Use the OTLP exporters you already have.
- **One codebase**: what you self-host is exactly what we run in production.
- **Built in Rust**: a small Docker image, low memory use, fast ingestion.

## Stack

| Component | Technology |
| --- | --- |
| Ingestion and API | Rust, `tonic` (gRPC), `axum` (HTTP) |
| Trace storage | ClickHouse |
| Control plane (orgs, API keys, config) | PostgreSQL |
| Quotas and rate limits | Redis |
| Web UI | TypeScript |

## Getting started

- **Source code**: [github.com/Comettrace/comettrace](https://github.com/Comettrace/comettrace)
- **Roadmap and issues**: [open issues](https://github.com/Comettrace/comettrace/issues)
- **Contributing**: start with issues labelled [`good first issue`](https://github.com/Comettrace/comettrace/labels/good%20first%20issue)

## Licence

The core is open source. Enterprise features are distributed under a separate commercial licence. See the main repository for details.

---

Questions, ideas or feedback: open an issue or a discussion on the main repository.
