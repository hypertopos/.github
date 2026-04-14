# hypertopos

A behavioral feature layer for graph and temporal data.

hypertopos turns relational data into a geometric coordinate space where:
- entities become positions
- relationships become structure
- behavior becomes movement
- anomalies become distance from the population

This layer sits between raw data and downstream systems:
- for exploration (analysts, agents)
- for feature generation (ML pipelines)
- for monitoring (drift, regime change)

No model training required.

## The stack

### [hypertopos-py](https://github.com/hypertopos/hypertopos-py)

Core engine. Transforms relational data into a geometric space where entities become coordinates, relationships become structure, and distance becomes signal.

### [hypertopos-mcp](https://github.com/hypertopos/hypertopos-mcp)

Agent interface. Exposes the geometric space as MCP tools — AI agents navigate, inspect, and reason about data structure directly.

### [hypertopos-skills](https://github.com/hypertopos/hypertopos-skills)

Investigation workflows. Structured behaviors that guide agents through real tasks: anomaly triage, fraud investigation, drift monitoring.

## How it fits together

Data → geometry ([hypertopos-py](https://github.com/hypertopos/hypertopos-py)) → tools ([hypertopos-mcp](https://github.com/hypertopos/hypertopos-mcp)) → reasoning ([hypertopos-skills](https://github.com/hypertopos/hypertopos-skills))

## Status

Research-stage project. Working code, reproducible benchmarks, active development. API may change.

`pip install hypertopos`
