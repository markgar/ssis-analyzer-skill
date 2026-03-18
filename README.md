# ssis-migration

SQL Server migration analysis plugins for [GitHub Copilot](https://github.com/features/copilot). Analyze SSIS packages and database schemas to plan and execute migrations to Azure.

> [!TIP]
> Each plugin can be installed independently — pick what you need.

## What's Included

| Plugin | Description |
|--------|-------------|
| [ssis-analyzer](plugins/ssis-analyzer/) | Analyze SSIS `.dtsx` packages — extract control flow, data flows, connections, variables, SQL, scripts, column lineage, and migration assessment. |
| [dacpac-analyzer](plugins/dacpac-analyzer/) | Analyze SQL Server `.dacpac` and `.bacpac` packages — extract tables, views, stored procedures, functions, constraints, indexes, schemas, and full database schema metadata. |

## Install a Plugin

```bash
copilot plugin marketplace add markgar/ssis-migration
copilot plugin install ssis-analyzer@ssis-migration
copilot plugin install dacpac-analyzer@ssis-migration
```

## Source

This collection is maintained at [markgar/ssis-migration](https://github.com/markgar/ssis-migration).

## License

MIT
