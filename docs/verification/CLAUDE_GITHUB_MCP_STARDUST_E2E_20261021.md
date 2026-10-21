# Stardust GitHub MCP — Claude/GPT isolated write acceptance

Recorded on 2026-10-21 (Asia/Taipei). Non-production credential-free fixture.

## Immutable target
- Repo: `s7310327-prog/stardust-hermes` (PUBLIC; independently maintained Stardust source tree)
- Base main HEAD when test branch was created: `af9249dfa712ef63d05642a98c61a1b7c8460b21`
- Test branch: `agent/claude/stardust-github-mcp-e2e-20261021`
- This fixture was created by **GPT's GitHub connector**, not Claude.
- No main merge, no PR, no workflow/deployment change, no application runtime modification.

## Claude.ai — complete with Claude's own `GitHub（shih-fo-dashboard 限定）` connector

**DO NOT treat a GPT-written fixture as proof of a Claude write.**

1. Read this fixture on the exact test branch using Claude's **authenticated** GitHub remote MCP. Identify connector name, repository, path, branch, and blob SHA.
2. On **this exact branch only**, create:
   `docs/verification/CLAUDE_GITHUB_MCP_STARDUST_RESULT_20261021.md`.
   Include: `CLAUDE_GITHUB_STARDUST_WRITE_E2E`, observed UTC time, repo/branch, connector tool names, this fixture blob SHA, created commit SHA (if available), and no secrets or personal data.
3. Independently GET the created file from GitHub. Prefer a **different read-only connector** for cross-connector verification. Compare exact content and blob SHA (full 40 hexadecimal characters), not a screenshot or a tool's "ok" boolean.
4. Return to owner/GPT: `CLAUDE_AUTH`, `CLAUDE_STARDUST_REPO_READ`, `CLAUDE_STARDUST_COMMIT_WRITE`, `CLAUDE_STARDUST_BLOB_READBACK`, `GITHUB_ACTOR`, exact 40-character commit/blob SHAs, and GitHub URLs. If authentication or write is denied, report the actual error; do **not** edit PAT scope or claim success.
5. Explicitly show that `main` remains unchanged and report whether the writing identity is the owner's PAT-backed account or an independent bot.

## Safety boundaries
- Do not change main, CI, Actions, credentials, source code, release, deployment, or production.
- Do not open or merge PRs as part of this microtest.
- Keep the result file limited to harmless verification metadata. No tokens, PATs, emails, API secrets, cookies, financial data, logs, or environment values.
- PUBLIC repo read access does **not** prove PAT access. The exact commit/GET is the positive **write** proof.
- Owner's explicit approval for this particular branch-only test does not authorize future unrestricted writes.

## States
- `GPT_STARDUST_WRITE_READBACK`: pending independent GPT readback of this fixture
- `CLAUDE_STARDUST_WRITE_E2E`: NOT_YET_VERIFIED until Claude completes step 2 and a separate GET confirms the resulting blob
