<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/broxhq/.github/main/profile/assets/logo-dark.svg">
  <img alt="brox" src="https://raw.githubusercontent.com/broxhq/.github/main/profile/assets/logo.svg" width="320">
</picture>

[![npm version](https://img.shields.io/npm/v/@broxhq/cli?label=%40broxhq%2Fcli&color=84cc16)](https://www.npmjs.com/package/@broxhq/cli)
[![qpilot](https://img.shields.io/npm/v/qpilot?label=qpilot&color=6366f1)](https://www.npmjs.com/package/qpilot)
[![license](https://img.shields.io/npm/l/@broxhq/cli?color=71717a)](https://github.com/broxhq/cli/blob/main/LICENSE)

</div>

---

## 🛩 qpilot

Paste a manual test case. An AI agent opens Chrome and executes each step — live `pass / fail / warn` per step. If it hits a captcha or OTP, it pauses and asks you directly.

```bash
npx qpilot
```

No code. No config. No Selenium. Just paste and run.

→ **[npmjs.com/package/qpilot](https://www.npmjs.com/package/qpilot)**

---

## Brox — package manager for AI agent skills

Self-contained bundles that extend what your agent can do. Think `npm` for Claude, Cursor, Cline, and Continue.

```bash
npm install -g @broxhq/cli

brox install @brox/pdf-extractor   # extract text from PDFs
brox install @brox/web-fetch       # fetch URLs as clean text
brox install @brox/git-context     # repo awareness for agents
brox install @brox/sqlite-query    # query .db files safely
```

Skills land in `.claude/skills/` — recognized by all major agents.

Browse all → [broxhq/registry](https://github.com/broxhq/registry)

---

## Repositories

| | |
|---|---|
| [**qpilot**](https://github.com/broxhq/qpilot) | AI agent that runs manual test cases in a real browser |
| [**cli**](https://github.com/broxhq/cli) | `@broxhq/cli` — the Brox package manager |
| [**registry**](https://github.com/broxhq/registry) | Public index of every skill |
| [**spec**](https://github.com/broxhq/spec) | The skill manifest format |
| [**examples**](https://github.com/broxhq/examples) | Reference skills, ready to install |

---

<div align="center">

[brox.sh](https://brox.sh) · [@broxhq on npm](https://www.npmjs.com/org/broxhq) · MIT

</div>
