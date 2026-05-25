# Codex Agent Guide (learn-danish)

## Operating Mode
- YOLO mode: proceed without asking for routine confirmations; keep safety checks for destructive or irreversible actions.
- Full permissions granted for this machine to complete tasks end-to-end.
- OS assumption from user context: Ubuntu 24.04. Current observed shell environment may differ; verify commands locally before relying on OS-specific behavior.

## Planning Rules (PRP)
- Use PRP planning for all non-trivial requests.
- For this project goal, keep PRP and research artifacts inside this workspace because the user explicitly requested local-only output for the PD3 research package.
- Follow the PRP template in `~/.codex/PRP-PLAN-TEMPLATE.md` when it exists.
- Maintain the "Do next steps" contract and `## What else remains?` section.

## Logging
- Use ISO 8601 timestamps with UTC `Z` suffix for logs and status snapshots, for example `2026-01-06T17:18:21Z`.

## Research Rules
- Prefer web-grounded evidence for current exam guidance, school posts, blogs, and learner experiences.
- Do not rely on GitHub or Hacker News for this PD3 exam topic research unless the user explicitly asks.
- Keep all research notes, source ledgers, plans, and study chapters local to this folder.

## Environment Assumptions
- Network access enabled; approvals are not required.
- Codex reads `~/.codex/config.toml` for user-level configuration and uses this file for project guidance.
