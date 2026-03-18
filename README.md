# ssis-analyzer-skill

A plugin repository for [GitHub Copilot](https://github.com/features/copilot) that provides SSIS package analysis capabilities.

## Plugins

| Plugin | Description |
|--------|-------------|
| [ssis-analyzer](plugins/ssis-analyzer/) | Analyze SSIS `.dtsx` packages — extract control flow, data flows, connections, variables, SQL, scripts, column lineage, and migration assessment. |

## Installation

```bash
copilot plugin marketplace add markgar/ssis-analyzer-skill
copilot plugin install ssis-analyzer@ssis-analyzer-skill
```

## Repository Structure

```
├── plugins/
│   └── ssis-analyzer/       # The plugin
│       ├── .github/plugin/  # Plugin manifest
│       ├── skills/          # Skills bundled with the plugin
│       ├── scripts/         # Python analysis scripts
│       └── README.md        # Plugin documentation
├── tests/                   # Test suite
└── pyproject.toml           # Python project config
```

## Development

```bash
# Run tests
pip install pytest
pytest tests/ -q
```

## License

MIT
