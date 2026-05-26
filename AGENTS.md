# Agent Guidelines

This document is for AI coding agents (Claude Code, Copilot, etc.).
Read this **before** making any changes to this repository.

---

## Project Overview

This is a GitHub profile README repository (`henry9904/henry9904`).
The only file that matters is `README.md` — it is rendered directly on the GitHub profile page.

---

## README Structure

The README has five fixed sections. Keep them in this order:

1. **Title + tagline** — one-line description of the owner's role
2. **Skills** — shields.io badges, split into "현재 사용 가능" and "학습 중"
3. **Projects** — markdown table with columns: 프로젝트 | 스택 | 설명
4. **Currently** — plaintext timeline inside a `text` code block
5. **Stats** — GitHub stats card (Vercel-hosted API)

---

## Rules

### Badges (Skills section)

Use shields.io `flat` style consistently:

```md
![Name](https://img.shields.io/badge/Label-COLOR?style=flat&logo=LOGO_ID&logoColor=white)
```

- Move a badge from "학습 중" to "현재 사용 가능" only when explicitly asked.
- Do not add badges for tools not mentioned by the owner.

### Projects table

- Link the project name to its GitHub URL.
- Keep the stack column concise (3–5 items max).
- Mark in-progress projects with `*(진행중)*` after the name.

### Currently section

- Entries are prefixed with `YYYY.MM ~`.
- Keep the indented continuation lines aligned with the first line's text start.
- Do not remove past entries unless explicitly asked.

### Stats card

The stats card URL uses the self-hosted Vercel deployment:

```
https://my-github-stats-two-alpha.vercel.app/api?username=henry9904&...
```

Do not change the base URL or the `username` parameter.

---

## What NOT to Do

- Do not add sections beyond the five listed above without being asked.
- Do not change the language of the README (Korean conventions are intentional).
- Do not modify the stats card query parameters without being asked.
