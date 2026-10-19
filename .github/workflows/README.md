# Workflows

| Workflow | Runs on | What it does |
| --- | --- | --- |
| [`config-lint.yml`](config-lint.yml) | Push to `main`, every pull request | Parses `settings.json` as JSON with comments and trailing commas, the way Zed reads it. Checks every `extensions.txt` line is `id@version` or a `//` comment |
| [`markdownlint.yml`](markdownlint.yml) | Push to `main`, every pull request | Lints every markdown file against [`.markdownlint.json`](../../.markdownlint.json) |

Both are also runnable manually via `workflow_dispatch` from the Actions tab.
