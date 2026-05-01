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
- **Prefix aliasing**: slash commands use the canonical `geno-` prefix in source (e.g., `/geno-upload-kaggle`). Short `/gt-` aliases are configured per-install by `geno-tools` and should not appear in skill definitions or documentation.

## Adding a new skill

1. Create `skills/<skill-name>/SKILL.md` with YAML front matter (`name`, `description`) and a `## Workflow` section.
2. Follow the naming convention: `geno-kaggle-<sub-skillset>-<skill>` (e.g., `geno-kaggle-benchmarks-task-generate`).
3. Add the skill to the table in GENO.md and to the umbrella SKILL.md.
4. Register the skill in `genotools.yaml` under the `skills` list.
5. Use agent-neutral language -- write "ask the user" or "prompt the user", never reference a specific tool name like `AskUserQuestion`.

## Dependencies and runtime

- [Kaggle CLI](https://github.com/Kaggle/kaggle-api) v2.0+ (`pip install kaggle`)
- Kaggle API credentials at `~/.kaggle/kaggle.json`
- No Python venv required (pure skill definitions, no runtime code)
