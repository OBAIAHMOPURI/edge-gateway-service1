# Edge Gateway Service 1 — Setup

[README](../README.md) · [Architecture](ARCHITECTURE.md)

## What can be done today

This is a documentation-first scaffold, not an installable application. Only a title-only README existed; no application source, build manifest, tests, or deployment configuration was present. The documentation adds no runtime implementation. Git and a Markdown viewer are sufficient to inspect the current project.

```sh
git clone https://github.com/OBAIAHMOPURI/edge-gateway-service1.git
cd edge-gateway-service1
git status
```

This repository contains documentation only after the documentation pass; no service is available to start.

## Runtime setup is not yet available

No language/runtime version, dependency lockfile, package manifest, build script, executable entry point, database migration, container definition, CI workflow, listening port, or health-check route has been selected or implemented. There is no `.env` loader. Do not assume `npm install`, `mvn package`, `docker compose up`, or a guessed HTTP endpoint will work.

## Proposed configuration contract — not consumed by current code

The names below are suggestions to discuss during implementation. They are **not working environment variables**, and no default values or secrets are provided.

| Candidate setting | Intended meaning |
| --- | --- |
| `UPSTREAM_ALLOWLIST` | Explicitly permitted synthetic/test upstreams |
| `ROUTING_POLICY_ID` | Versioned policy selected for the experiment |
| `REQUEST_TIMEOUT_MS` | Tested request budget; value not yet chosen |

Actual configuration must document required/optional fields, validation, source of secrets, safe local values, failure behavior for missing values, and how the application reads them. Use sandbox credentials obtained through an approved channel, not copied from public examples.

## Implementation-readiness checklist

- [ ] Approve the repository's exact responsibility and its relationships to siblings.
- [ ] Select a supported runtime/framework and pin dependency/build versions.
- [ ] Add source, an executable entry point, and a reproducible local start/stop command.
- [ ] Implement and document input/output contracts and required local dependencies.
- [ ] Add synthetic fixtures, unit tests, and sandbox integration/failure tests.
- [ ] Document configuration loading, secret handling, resource limits, retries, and recovery.
- [ ] Add a health/readiness interface only if appropriate, with an exact documented route.
- [ ] Record one verified local build/run transcript before advertising a runnable quick start.

## Service-specific first decisions

- Choose whether this remains an experiment, becomes the canonical gateway, or is retired through a separately approved change.
- Record the concrete design difference from edge-gateway-service; none is currently verified.
- Select a runtime and define a reproducible local evaluation before promising performance or compatibility.

## Validation and troubleshooting

At present, a missing build file or executable is expected, not an installation failure. Review the current tree before installing software. Once code exists, update this guide with the exact working prerequisites, commands, expected outputs, and actual error recovery. This documentation pass performed static inspection only; it did not start services, send alerts, synchronize external systems, or verify integrations.
