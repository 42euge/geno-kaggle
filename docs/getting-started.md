# Getting Started

## Prerequisites

- A supported coding CLI (Claude Code, Gemini CLI, Codex, or OpenCode)
- [geno-tools](https://github.com/42euge/geno-tools) installed
- [Kaggle CLI](https://github.com/Kaggle/kaggle-api) v2.0+ (`pip install kaggle`)
- Kaggle API credentials at `~/.kaggle/kaggle.json`

## Install

```bash
geno-tools install geno-kaggle
```

Or from within an agent session:

```
/geno-tools install geno-kaggle
```

## First use

Once installed, the geno-kaggle skills are available as slash commands in your agent session.

### Create a benchmark notebook

```
/geno-create-benchmark-kaggle attention "selective attention with distractor scaling"
```

### Run a benchmark on Kaggle

```
/geno-run-kaggle-bench tasks/attention_benchmark.ipynb
```

### Scrape competition discussions

```
/geno-kaggle-discussion
```
