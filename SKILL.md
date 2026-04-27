---
name: geno-kaggle
description: >-
  Kaggle benchmarking toolkit — create, run, monitor, and review benchmark notebooks
  on the Kaggle platform. Scrape competition discussions for insights.
  Use when user says /geno-kaggle-*, /geno-run-kaggle-bench, /geno-upload-kaggle,
  or /geno-create-benchmark-kaggle.
license: MIT
metadata:
  author: 42euge
  version: "0.1.0"
---

# geno-kaggle

Kaggle benchmarking skills for AI coding agents. Provides workflows for creating, deploying,
running, and reviewing benchmark tasks on the Kaggle platform.

## Skills

| Skill | Description |
|-------|-------------|
| `/geno-create-benchmark-kaggle <desc>` | Create a self-contained benchmark notebook for Kaggle |
| `/geno-kaggle-benchmarks-task-generate <name>` | Scaffold a new benchmark task folder structure |
| `/geno-kaggle-benchmarks-task-review <task>` | Pull and review results from a Kaggle benchmark run |
| `/geno-run-kaggle-bench <notebook>` | Push, run, monitor, and debug a notebook on Kaggle |
| `/geno-upload-kaggle <notebook>` | Upload a notebook to Kaggle |
| `/geno-kaggle-discussion` | Scrape competition discussions and generate insights |
