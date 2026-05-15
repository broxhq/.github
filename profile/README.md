<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/broxhq/.github/main/profile/assets/logo-dark.svg">
  <img alt="brox" src="https://raw.githubusercontent.com/broxhq/.github/main/profile/assets/logo.svg" width="320">
</picture>

### The package manager for AI agent skills.

[![npm version](https://img.shields.io/npm/v/@broxhq/cli?label=%40broxhq%2Fcli&color=84cc16)](https://www.npmjs.com/package/@broxhq/cli)
[![license](https://img.shields.io/npm/l/@broxhq/cli?color=71717a)](https://github.com/broxhq/cli/blob/main/LICENSE)
[![registry](https://img.shields.io/badge/registry-broxhq%2Fregistry-0a0a0a)](https://github.com/broxhq/registry)

</div>

---

## What is Brox?

Brox is a package manager for **AI agent skills** — self-contained bundles of instructions, scripts, and references that extend what your agent can do.

Think of it as `npm` for Claude, Cursor, Cline, Continue, and any agent that follows the [Agent Skills](https://github.com/broxhq/spec) convention.

```bash
npm install -g @broxhq/cli

brox search pdf                          # find a skill
brox install @brox/pdf-extractor         # install it
brox list                                # see what's installed
brox init                                # create your own
```

Skills land in `./.claude/skills/` (per-project) or `~/.claude/skills/` (global) — the convention recognized by all major agents.

## Featured skills

| Skill | What it does |
|-------|--------------|
| [`@brox/pdf-extractor`](https://github.com/broxhq/examples/tree/main/pdf-extractor) | Extract text from PDFs. Pure Python (only needs `pypdf`). |
| [`@brox/web-fetch`](https://github.com/broxhq/examples/tree/main/web-fetch) | Fetch a URL and return clean readable text. Python stdlib only. |
| [`@brox/git-context`](https://github.com/broxhq/examples/tree/main/git-context) | Give the agent fast situational awareness of any repo. |
| [`@brox/sqlite-query`](https://github.com/broxhq/examples/tree/main/sqlite-query) | Inspect schema and run SQL queries against `.db` files safely. |

Browse the full list at [broxhq/registry](https://github.com/broxhq/registry).

## Repositories

| | |
|---|---|
| [**cli**](https://github.com/broxhq/cli) | `@broxhq/cli` — the package manager itself |
| [**registry**](https://github.com/broxhq/registry) | Public index of every skill; PRs validated and auto-merged |
| [**spec**](https://github.com/broxhq/spec) | The skill manifest format and JSON schema |
| [**examples**](https://github.com/broxhq/examples) | Reference skills, ready to install |

## Publishing your own skill

```bash
brox init           # scaffold a new skill
# edit SKILL.md and add scripts, then commit to your GitHub repo
brox login          # authenticate with GitHub (Device Flow)
brox publish        # tag, push, fork registry, open PR
```

You publish under your own GitHub username as the scope: if you're `alice`, `@alice/*` is yours. CI validates the PR against [these checks](https://github.com/broxhq/registry/blob/main/scripts/validate.py) and auto-merges on success — usually in under a minute.

## Get involved

- ⭐ Star the repos you use — it helps others discover Brox
- 🛠 Build a skill and `brox publish` it
- 🐛 Report bugs in the relevant repo
- 🌐 Website: [brox.sh](https://brox.sh)

---

<div align="center">

[brox.sh](https://brox.sh) · [@broxhq on npm](https://www.npmjs.com/org/broxhq) · MIT licensed

</div>
