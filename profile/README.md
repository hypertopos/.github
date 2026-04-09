# hypertopos

**Your data has shape. We help AI agents find it.**

hypertopos turns relational data into navigable geometric space. Every entity gets a polygon built from its relationships — and that shape reveals anomalies, drift, clusters, and structure that SQL cannot see.

## Packages

| Package | What it does | Install |
|---------|-------------|---------|
| [**hypertopos-py**](https://github.com/hypertopos/hypertopos-py) | Core library — 12 navigation primitives, Arrow IPC storage, unsupervised detection | `pip install hypertopos` |
| [**hypertopos-mcp**](https://github.com/hypertopos/hypertopos-mcp) | 55 MCP tools — AI agents explore spheres through geometry, not SQL | `pip install hypertopos-mcp` |
| [**hypertopos-skills**](https://github.com/hypertopos/hypertopos-skills) | 8 agent playbooks — investigation, exploration, fraud detection, sphere design | `npx skills add hypertopos/hypertopos-skills` |

## Validated on real data

| Domain | Dataset | Result |
|--------|---------|--------|
| Banking | Berka (real Czech banking) | 85.5–90.8% recall, unsupervised |
| Transportation | NYC Yellow Taxi (7.6M trips) | 8/8 anomaly categories |
| AML | IBM AML (5M transactions) | 80.4% recall, FP/TP=0.6 |

## Links

- [hypertopos.com](https://hypertopos.com)
- [DOI: 10.5281/zenodo.19482069](https://doi.org/10.5281/zenodo.19482069)
