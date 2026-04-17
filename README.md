# geno-kaggle

Kaggle benchmarking skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code). Create, run, monitor, and review benchmark tasks on the Kaggle platform.

## Commands

| Command | Description |
|---------|-------------|
| `/gt-create-benchmark-kaggle <desc>` | Create a self-contained benchmark notebook for Kaggle |
| `/gt-kaggle-benchmarks-task-generate <name>` | Scaffold a new benchmark task folder structure |
| `/gt-kaggle-benchmarks-task-review <task>` | Pull and review results from a Kaggle benchmark run |
| `/gt-run-kaggle-bench <notebook>` | Push, run, monitor, and debug a notebook on Kaggle |
| `/gt-upload-kaggle <notebook>` | Upload a notebook to Kaggle |
| `/gt-kaggle-discussion` | Scrape competition discussions and generate insights |

## Prerequisites

- [Kaggle CLI](https://github.com/Kaggle/kaggle-api) v2.0+ (`pip install kaggle`)
- Kaggle API credentials at `~/.kaggle/kaggle.json`

## Install

```bash
./install.sh
```

Or install via geno-tools ecosystem installer:
```bash
cd ../geno-tools && ./install.sh
```

## Part of the geno ecosystem

- [geno-tools](https://github.com/42euge/geno-tools) — orchestrator + general tools
- [geno-research](https://github.com/42euge/geno-research) — deep research workflows
- [geno-media](https://github.com/42euge/geno-media) — media creation (audiobooks, video)

## License

MIT
