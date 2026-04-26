# geno-kaggle

Kaggle benchmarking toolkit for AI coding agents -- create, run, monitor, and review benchmark notebooks on the Kaggle platform, and scrape competition discussions for insights.

## Skills

| Skill | Sub-skillset | Slash command |
|-------|-------------|---------------|
| geno-kaggle | -- | -- (umbrella) |
| geno-create-benchmark-kaggle | benchmarks | /geno-create-benchmark-kaggle |
| geno-kaggle-benchmarks-task-generate | benchmarks | /geno-kaggle-benchmarks-task-generate |
| geno-kaggle-benchmarks-task-review | benchmarks | /geno-kaggle-benchmarks-task-review |
| geno-kaggle-discussion | discussions | /geno-kaggle-discussion |
| geno-run-kaggle-bench | benchmarks | /geno-run-kaggle-bench |
| geno-upload-kaggle | uploads | /geno-upload-kaggle |

## Repo structure

```
geno-kaggle/
├── GENO.md              # agent instructions (this file)
├── SKILL.md             # umbrella skill manifest
├── genotools.yaml       # geno-tools manifest
├── skills/              # skill definitions
│   ├── geno-kaggle/     #   umbrella
│   ├── geno-create-benchmark-kaggle/
│   ├── geno-kaggle-benchmarks-task-generate/
│   ├── geno-kaggle-benchmarks-task-review/
│   ├── geno-kaggle-discussion/
│   ├── geno-run-kaggle-bench/
│   └── geno-upload-kaggle/
├── commands/            # legacy command files (gt-*.md)
├── config/              # default config templates
│   └── defaults/
│       └── colab.json
├── docs/                # documentation site
│   ├── index.md
│   └── getting-started.md
└── mkdocs.yml           # MkDocs Material config
```

## Conventions

- **Skill files**: each skill lives in `skills/<skill-name>/SKILL.md`
- **Skill naming**: follows the geno ecosystem `{skillset}-{sub-skillset}-{skill}` convention
- **Install method**: `geno-tools install geno-kaggle` (canonical), never `./install.sh` or `npx skills add`
- **Agent-neutral language**: descriptions use "coding agent" / "agent session", not a specific agent name

## Dependencies and runtime

- [Kaggle CLI](https://github.com/Kaggle/kaggle-api) v2.0+ (`pip install kaggle`)
- Kaggle API credentials at `~/.kaggle/kaggle.json`
- No Python venv required (pure skill definitions, no runtime code)
