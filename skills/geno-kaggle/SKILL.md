---
name: geno-kaggle
description: >-
  Kaggle benchmarking toolkit — create, run, monitor, and review benchmark notebooks
  on the Kaggle platform. Scrape competition discussions for insights.
  Use when user says /gt-kaggle-*, /gt-run-kaggle-bench, /gt-upload-kaggle,
  or /gt-create-benchmark-kaggle.
license: MIT
metadata:
  author: 42euge
  version: "0.1.0"
---

# geno-kaggle

Kaggle benchmarking skills for Claude Code. Provides workflows for creating, deploying,
running, and reviewing benchmark tasks on the Kaggle platform.

## Commands

| Command | Description |
|---------|-------------|
| `/gt-create-benchmark-kaggle <desc>` | Create a self-contained benchmark notebook for Kaggle |
| `/gt-kaggle-benchmarks-task-generate <name>` | Scaffold a new benchmark task folder structure |
| `/gt-kaggle-benchmarks-task-review <task>` | Pull and review results from a Kaggle benchmark run |
| `/gt-run-kaggle-bench <notebook>` | Push, run, monitor, and debug a notebook on Kaggle |
| `/gt-upload-kaggle <notebook>` | Upload a notebook to Kaggle |
| `/gt-kaggle-discussion` | Scrape competition discussions and generate insights |
