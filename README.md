# geno-kaggle

Kaggle benchmarking skills for AI coding agents. Create, run, monitor, and review benchmark tasks on the Kaggle platform.

## Skills

| Skill | Description |
|-------|-------------|
| `/geno-create-benchmark-kaggle <desc>` | Create a self-contained benchmark notebook for Kaggle |
| `/geno-kaggle-benchmarks-task-generate <name>` | Scaffold a new benchmark task folder structure |
| `/geno-kaggle-benchmarks-task-review <task>` | Pull and review results from a Kaggle benchmark run |
| `/geno-run-kaggle-bench <notebook>` | Push, run, monitor, and debug a notebook on Kaggle |
| `/geno-upload-kaggle <notebook>` | Upload a notebook to Kaggle |
| `/geno-kaggle-discussion` | Scrape competition discussions and generate insights |

## Prerequisites

- [Kaggle CLI](https://github.com/Kaggle/kaggle-api) v2.0+ (`pip install kaggle`)
- Kaggle API credentials at `~/.kaggle/kaggle.json`
- A supported coding CLI (Claude Code, Gemini CLI, Codex, or OpenCode)

## Install

```bash
geno-tools install geno-kaggle
```

Or from within an agent session:

```
/geno-tools install geno-kaggle
```

## Part of the geno ecosystem

- [geno-tools](https://github.com/42euge/geno-tools) — orchestrator + general tools
- [geno-research](https://github.com/42euge/geno-research) — deep research workflows
- [geno-media](https://github.com/42euge/geno-media) — media creation (audiobooks, video)

## License

MIT
