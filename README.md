# @riotprompt/riotplan-commands-render

Render commands for RiotPlan CLI. Export plans to Markdown, JSON, and HTML formats.

## Installation

```bash
npm install @riotprompt/riotplan-commands-render
```

## Commands

### render

Render a plan to various formats.

```bash
riotplan render [options]
```

**Options:**
- `-p, --path <path>` - Path to plan directory (default: ".")
- `-f, --format <format>` - Output format: markdown, json, html (default: "markdown")
- `-o, --output <file>` - Output file (defaults to stdout)
- `--theme <theme>` - HTML theme: light, dark (default: "light")
- `--pretty` - Pretty print JSON output
- `--no-metadata` - Exclude metadata from output
- `--feedback` - Include feedback records
- `--evidence` - Include evidence records
- `--task-list` - Use task list format for markdown steps
- `--toc` - Include table of contents (markdown)
- `--no-styles` - Exclude styles from HTML output
- `--full` - Include all details

## Usage

```typescript
import { registerRenderCommands } from "@riotprompt/riotplan-commands-render";
import { Command } from "commander";

const program = new Command();
registerRenderCommands(program);
```

## License

Apache-2.0

<!-- v1.0.0 -->

