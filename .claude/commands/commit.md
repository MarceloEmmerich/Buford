
# Commit Changes

Your job is to create clean, atomic git commits based on the specification work done in this session.

## Context

- You have access to `specs/` which documents session progress.
- You must use conversation history + `git status` + `git diff` to understand what has changed.
- Your commits must follow the principles below.

## Principles

1. **Atomic commits**: Group logically related changes together.
2. **Imperative messages**: Write commit messages in imperative mood (e.g., "Add X", "Update Y", "Refactor Z").
3. **Focus on why**: Capture the intent and reasoning for the change, not just the mechanical edits.
4. **User ownership**: Commits are authored solely by the user. Never attribute to Claude or any AI.

## Process

1. **Review changes**
   - Run `git status` to see modified/new files
   - Run `git diff` to understand modifications
   - Cross-check against `specs/` to see what was requested

2. **Draft commit plan**
   - Decide how many commits are appropriate
   - For each commit, list the files to add
   - Write a descriptive commit message

3. **Confirm with user**
   - Present the commit plan clearly
   - Ask: *"I plan to create [N] commit(s) with these changes. Shall I proceed?"*

4. **Execute upon confirmation**
   - Stage files individually: `git add path/to/file`
   - Commit with planned message: `git commit -m "Message"`
   - Show result with `git log --oneline -n [N]`

## Constraints

- Never use `git add -A` or `git add .`
- Never include "Generated with Claude" or "Co-Authored-By"
- Never skip confirmation before committing
- Assume timestamps are managed by `git` and do not alter them

---

