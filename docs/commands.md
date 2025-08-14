# Commands

This page lists all available **DAI CLI** commands and their usage.

---

## `dai auth`

Authenticate DAI with external services (currently GitHub token only).

```bash
dai auth
```

Prompts for a GitHub Personal Access Token (PAT) and saves it in the local configuration.

---

## `dai completion`

Generate the autocompletion script for your shell.

```bash
dai completion bash
dai completion zsh
dai completion fish
```

---

## `dai config`

Configure global DAI settings stored in `~/.dai/config.yaml`.

```bash
dai config
```

---

## `dai ignore`

Create a default `.daiignore` file in the project root (uses `.gitignore` syntax).

```bash
dai ignore
```

---

## `dai init`

Initialize DAI for the current project by creating `.dai/project.yaml`.

```bash
dai init
```

---

## `dai triage`

Analyze a commit and open a single GitHub issue with findings.

```bash
dai triage --commit <commit_hash>
```

Options:
- `--commit` — Commit hash to analyze (defaults to the latest commit)

---

## `dai triage-local`

Analyze a single local file and append findings to `.dai/local.log`.

```bash
dai triage-local path/to/file.go
```

---

## Global Flags

| Flag                  | Description                                             |
|-----------------------|---------------------------------------------------------|
| `-h, --help`          | Show help for a command                                 |
| `-p, --parrot string` | Summon the DAI parrot (`party`, `insult`, `wise` modes) |
| `-v, --version`       | Show the DAI version                                    |

---

Next: [Troubleshooting](troubleshooting.md)
