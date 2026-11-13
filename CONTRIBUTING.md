# Contributing to Edge Gateway Service 1

[Root README](README.md) · [Architecture](docs/ARCHITECTURE.md) · [Setup](docs/SETUP.md) · [API guide](docs/API.md) · [Network Ecosystem](README.md#network-ecosystem)

## Project status and scope decision

This is a documentation-only gateway candidate. The suffix `1` does not establish a version, fork, replacement, or deployment relationship to `edge-gateway-service`. No runtime implementation, manifest, listener, or automated test suite exists. Resolve the intended scope with the owner before implementing or claiming compatibility.

## Local contribution workflow

```sh
git clone https://github.com/OBAIAHMOPURI/edge-gateway-service1.git
cd edge-gateway-service1
git switch -c docs/describe-change
```

Read the linked guides, agree a small change and acceptance criteria, and use a focused pull request for normal review. Explicit direct-to-main approval for this documentation batch is not a standing merge policy. Do not invent package-manager commands, install dependencies, or rename/merge either gateway as incidental cleanup.

## Repository-specific priorities

- Decide whether this is an experiment, an independent gateway, the canonical implementation, or a candidate for separately approved retirement.
- Document a concrete design difference and measurable correctness/failure criteria before comparing it with the other gateway.
- Define approved synthetic upstreams, route/policy contracts, header trust rules, timeout budgets, and safe request retry behavior.
- Choose a supported runtime and reproducible local evaluation harness before performance or compatibility claims.

## Quality and evidence

Documentation changes should run `git diff --check`, render Markdown, preserve exact repository casing, and verify root README/architecture/setup/API backlinks and every sibling link. Label proposed behavior explicitly and do not claim tests or integrations that do not exist.

Future code should add synthetic fixtures and tests for invalid routing configuration, rejected destinations, upstream failures, identity/header spoofing, policy parity only where intended, timeout/cancellation, and isolation from live services. Report the actual commands, versions, results, and unrun checks. Pull requests should explain scope, rationale, compatibility, evidence, unresolved decisions, and rollback/migration needs; update contracts and setup instructions with implementation changes.

## Safety and ownership

Never commit credentials, tokens, private operational notes, or real request payloads. Use sandbox traffic only. Sensitive reports belong in an owner-approved private channel. Production proxying, live infrastructure, access changes, and repository retirement require separate authorization. No license is selected or granted by this guide.

## Sibling repository network

Documentation navigation only; no live network integration or gateway hierarchy is claimed.

- [alert-notification-dispatcher](https://github.com/OBAIAHMOPURI/alert-notification-dispatcher/blob/main/README.md)
- [Brainwave_Matrix_Intern — Banky Application](https://github.com/OBAIAHMOPURI/Brainwave_Matrix_Intern/blob/main/README.md)
- [BrainWave_Matrix_Intern1 — Hospital Management System](https://github.com/OBAIAHMOPURI/BrainWave_Matrix_Intern1/blob/main/README.md)
- [edge-gateway-service](https://github.com/OBAIAHMOPURI/edge-gateway-service/blob/main/README.md)
- [identity-auth-proxy](https://github.com/OBAIAHMOPURI/identity-auth-proxy/blob/main/README.md)
- [telemetry-stream-worker](https://github.com/OBAIAHMOPURI/telemetry-stream-worker/blob/main/README.md)
- [workflow-state-sync](https://github.com/OBAIAHMOPURI/workflow-state-sync/blob/main/README.md)
