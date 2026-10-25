# hypertopos

Business data as geometry that AI agents navigate.

hypertopos turns relational data into a shared geometric space where:
- entities become positions, derived from their relationships and the population around them
- relationships become structure
- behavior becomes movement
- anomalies become distance from the population — and the direction of that distance explains them

It complements SQL: the database answers *which rows match*; hypertopos answers *which entities are out of place, how that is changing, and why*.

This layer sits between raw data and downstream systems:
- for exploration (analysts, agents)
- for feature generation (ML pipelines)
- for monitoring (drift, regime change)

No model training required.

## The stack

### [hypertopos-py](https://github.com/hypertopos/hypertopos-py)

Core engine. Builds a sphere from a YAML description and stores it as Lance datasets. Every session reads one consistent snapshot while builds, ingests and recalibrations continue underneath; what-if work — a recalibration without suspected influencers, a trial ingest — runs on a copy-free branch that is compared with main, then promoted or deleted.

### [hypertopos-mcp](https://github.com/hypertopos/hypertopos-mcp)

Agent interface. Exposes the sphere as MCP tools — AI agents navigate, inspect, and reason about data structure directly. Runs as a local stdio server or as a hosted HTTP service with an independent session per connected agent; responses are compact JSON built for an agent's context window.

### [hypertopos-skills](https://github.com/hypertopos/hypertopos-skills)

Investigation workflows. Structured behaviors that guide agents through real tasks: anomaly triage, root-cause tracing, chain and fraud investigation, drift monitoring, sphere design.

## How it fits together

Data → geometry ([hypertopos-py](https://github.com/hypertopos/hypertopos-py)) → tools ([hypertopos-mcp](https://github.com/hypertopos/hypertopos-mcp)) → reasoning ([hypertopos-skills](https://github.com/hypertopos/hypertopos-skills))

## Status

Research-stage project. Working code, reproducible benchmarks, active development. API may change.

`pip install hypertopos`
