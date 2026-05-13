# cc-plugins

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Personal [Claude Code](https://claude.ai/code) plugin marketplace by [Alexandre Roman](https://github.com/alexandreroman).

## Installation

```bash
# In Claude Code
/plugin marketplace add alexandreroman/cc-plugins
```

Or as a local directory (for development):

```bash
/plugin marketplace add /Users/alex/Projects/cc-plugins
```

## Available plugins

| Plugin     | Description                                                        | Source                                                                      |
| ---------- | ------------------------------------------------------------------ | --------------------------------------------------------------------------- |
| `cmux`     | Integrates Claude Code with [cmux](https://www.cmux.dev) terminal. | [alexandreroman/cmux-plugin](https://github.com/alexandreroman/cmux-plugin) |
| `skillbox` | Repository of reusable skills and agents for Claude Code.          | [alexandreroman/skillbox](https://github.com/alexandreroman/skillbox)       |

## Installing a plugin

```bash
/plugin install <plugin-name>@cc-plugins
/reload-plugins
```

For example:

```bash
/plugin install cmux@cc-plugins
```

## Structure

```
cc-plugins/
└── .claude-plugin/
    └── marketplace.json   # Plugin registry
```

Each plugin entry references its source GitHub repository — this marketplace doesn't host plugin code, only the index.

## License

MIT
