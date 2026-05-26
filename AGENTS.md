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

---

## AI Agent Mistakes Log

이 섹션은 AI 에이전트가 이 레포에서 실수한 내용을 기록합니다.
새로운 실수를 발견하면 아래에 추가하세요.

형식:
```
### YYYY-MM-DD — Agent: [이름]
**실수**: 무슨 일이 있었는지
**영향**: 어떤 문제가 생겼는지
**수정**: 어떻게 고쳤는지
**교훈**: 다음에 뭘 확인해야 하는지
```

---

### 2026-05-26 — Agent: Claude Code

**실수**: AGENTS.md를 작성할 때 README의 실제 현재 내용을 확인하지 않고 이전 버전 기준으로 작성함. 오너가 직접 README를 "Henry | Data Engineer" → "Crong | Data Engineer"로 수정했으나 AGENTS.md에는 반영되지 않음.

**영향**: AGENTS.md의 가이드라인이 실제 README 내용과 불일치. 에이전트가 오래된 정보를 기준으로 작업할 위험.

**수정**: 없음 (타이틀 자체는 AGENTS.md 본문에 명시하지 않아 큰 영향 없음. 단, 구조 가이드라인은 여전히 유효).

**교훈**: README 구조 가이드라인을 쓰기 전에 반드시 현재 README를 읽고 시작할 것. 오너가 직접 수정할 수 있으므로 항상 최신 상태를 먼저 확인.
