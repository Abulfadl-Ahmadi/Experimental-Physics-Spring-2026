---
name: git-commit
description: 'Execute git commit with conventional commit message analysis, intelligent staging, and message generation. Use when user asks to commit changes, create a git commit, or mentions "/commit". Supports: (1) Auto-detecting type and scope from changes, (2) Generating conventional commit messages from diff, (3) Interactive commit with optional type/scope/description overrides, (4) Intelligent file staging for logical grouping'
license: MIT
allowed-tools: Bash
---

# Git Commit with Conventional Commits

## Overview

Create standardized, semantic git commits using the Conventional Commits specification. Analyze the actual diff to determine appropriate type, scope, and message.

## Conventional Commit Format

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

## Commit Types

| Type       | Purpose                        |
| ---------- | ------------------------------ |
| `feat`     | New feature                    |
| `fix`      | Bug fix                        |
| `docs`     | Documentation only             |
| `style`    | Formatting/style (no logic)    |
| `refactor` | Code refactor (no feature/fix) |
| `perf`     | Performance improvement        |
| `test`     | Add/update tests               |
| `build`    | Build system/dependencies      |
| `ci`       | CI/config changes              |
| `chore`    | Maintenance/misc               |
| `revert`   | Revert commit                  |

## Breaking Changes

```
# Exclamation mark after type/scope
feat!: remove deprecated endpoint

# BREAKING CHANGE footer
feat: allow config to extend other configs

BREAKING CHANGE: `extends` key behavior changed
```

## Workflow

### 1. Analyze Diff

```bash
# If files are staged, use staged diff
git diff --staged

# If nothing staged, use working tree diff
git diff

# Also check status
git status --porcelain
```

### 2. Stage Files (if needed)

If nothing is staged or you want to group changes differently:

```bash
# Stage specific files
git add path/to/file1 path/to/file2

# Stage by pattern
git add *.test.*
git add src/components/*

# Interactive staging
git add -p
```

**Pre-flight secret detection (do this BEFORE staging):**

```bash
# Scan untracked/staged files for common secret patterns
git status --porcelain | grep -iE '\.(env|pem|key)$|credential|secret|\.npmrc|api.?key|\.p12$'
```

If sensitive files are found:
1. Add them to `.gitignore` first.
2. Verify exclusion with `git check-ignore <file>` (should echo the filename back).
3. Commit the `.gitignore` change as a separate `chore:` commit -- never bundle it with feature work.

**Never commit secrets** (.env, credentials.json, private keys, `*.pem`, `*.key`).

### 3. Generate Commit Message

Analyze the diff to determine:

- **Type**: What kind of change is this?
- **Scope**: What area/module is affected?
- **Description**: One-line summary of what changed (present tense, imperative mood, <72 chars)

### 4. Execute Commit

```bash
# Single line
git commit -m "<type>[scope]: <description>"

# Multi-line with body/footer
git commit -m "$(cat <<'EOF'
<type>[scope]: <description>

<optional body>

<optional footer>
EOF
)"
```

## Best Practices

- One logical change per commit
- Present tense: "add" not "added"
- Imperative mood: "fix bug" not "fixes bug"
- Reference issues: `Closes #123`, `Refs #456`
- Keep description under 72 characters

## User Preference: Granular Commits Over One Mega-Commit

**This user explicitly prefers multiple small, logical commits over a single large commit** for a batch of related changes ("بهتر همه رو داخل یک کامینت نذاری و چندین تا کامیت محتلف بزنی — اینجوری استانداردتر و حرفه‌ای‌تر هست"). Honor this by default — they read git history as documentation.

**Workflow for a large batch:**
1. Keep changes uncommitted (or `git reset --soft <last-commit>`) so they form one unit.
2. Split by logical unit and commit each separately. Example split for a vault build:
   - `chore:` config/text sweeps (e.g. midterm→final, .gitignore)
   - `feat:` synthesis notes (Wiki hubs, profiles, methods)
   - `feat:` index/tracker notes (Journal)
   - `feat:` source-file patches (wikilink nav blocks)
   - `feat:` root README + Brain-Map
3. Verify with `git log --oneline` that history reads as a clean, reviewable sequence.

**Pitfall:** Do NOT squash a multi-note/source ingestion into one `feat:` commit just because it's faster. Granular commits are the deliverable, not a chore.

### 5. Verify

After committing, verify the result:

```bash
# Confirm the commit landed and message reads well
git log --oneline -5

# Confirm clean working tree (no stray files left behind)
git status

# If .gitignore was updated, confirm secret files are excluded
git check-ignore .env   # should echo ".env" back
```

## Git Safety Protocol

- NEVER update git config
- NEVER run destructive commands (--force, hard reset) without explicit request
- NEVER skip hooks (--no-verify) unless user asks
- NEVER force push to main/master
- If commit fails due to hooks, fix and create NEW commit (don't amend)
