# DACPAC Analyzer Plugin

Analyze SQL Server `.dacpac` and `.bacpac` package files — extract tables, views,
stored procedures, functions, constraints, indexes, schemas, sequences, table types,
roles, permissions, and all SQL body scripts.

## Installation

```bash
# Using Copilot CLI
copilot plugin install dacpac-analyzer@ssis-migration
```

Or register the marketplace first:

```bash
copilot plugin marketplace add markgar/ssis-migration
copilot plugin install dacpac-analyzer@ssis-migration
```

## What's Included

### Skills

| Skill | Description |
|-------|-------------|
| `dacpac-analyzer` | Analyze `.dacpac` and `.bacpac` packages to document database schema, extract SQL scripts, search objects, and audit constraints and indexes. |

### Commands (Slash Commands)

| Command | Description |
|---------|-------------|
| `overview` | Package metadata, origin info, and object counts |
| `summary` | High-level stats — counts per object type |
| `list-schemas` | All database schemas |
| `list-tables` | All tables with column counts |
| `table-detail` | Full table — columns, types, nullability, constraints, indexes |
| `list-views` | All views with column counts |
| `view-detail` | View columns and query script |
| `list-procedures` | All stored procedures |
| `procedure-detail` | Procedure parameters, body script, dependencies |
| `list-functions` | All functions (scalar + inline TVF) |
| `function-detail` | Function parameters, return type, body script |
| `list-constraints` | All PKs, FKs, unique, check, and default constraints |
| `list-indexes` | All indexes with columns and type |
| `list-sequences` | All sequences with type, start, increment |
| `list-table-types` | All user-defined table types |
| `list-roles` | All database roles |
| `list-permissions` | All permission statements |
| `extract-sql` | All SQL body scripts from views, procedures, functions |
| `find` | Case-insensitive search across all named objects and columns |

## Key Features

- **Full schema extraction** — tables, views, stored procedures, functions, and all object types
- **Constraint and index audit** — PKs, FKs, unique, check, default constraints, and indexes
- **SQL script extraction** — pull body scripts from views, procedures, and functions
- **Object search** — case-insensitive search across all named objects and columns
- **Schema metadata** — schemas, sequences, table types, roles, and permissions
- **DACPAC and BACPAC support** — works with both package formats

## Requirements

- Python 3.10+
- No external dependencies (pure Python standard library)

## Source

This plugin is published from [markgar/ssis-migration](https://github.com/markgar/ssis-migration).

## License

MIT
