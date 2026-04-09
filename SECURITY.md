# Security Policy

## Supported Versions

| Package | Version | Supported |
|---------|---------|-----------|
| [hypertopos](https://github.com/hypertopos/hypertopos-py) | 0.1.x | Yes |
| [hypertopos-mcp](https://github.com/hypertopos/hypertopos-mcp) | 0.1.x | Yes |
| [hypertopos-skills](https://github.com/hypertopos/hypertopos-skills) | 0.1.x | Yes |

## Architecture

All hypertopos packages run **locally**. No network services, no auth layer, no multi-tenancy.

### What to watch for

- **Pickle files** — chain cache (`.cache/chains_*.pkl`) uses pickle. Don't load cache files from untrusted sources.
- **Sphere paths** — `HyperSphere.open(path)` reads from the local filesystem. Don't point it at user-controlled paths without validation.
- **MCP server** — communicates over stdio. Not designed for network exposure.

## Reporting a Vulnerability

Use [GitHub private vulnerability reporting](https://github.com/hypertopos/hypertopos-py/security/advisories/new) or email [contact@hypertopos.com](mailto:contact@hypertopos.com).
