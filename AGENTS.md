# Kervra - Agent Instructions

## 1. Project Identity

Kervra is an open-source, local-first fitness and wellness application built
with Flutter and Dart for Android and iOS.

The product principle is:

"Strength, built daily."

Prioritize correctness, privacy, accessibility, maintainability, and a
polished user experience.

## 2. Git and GitHub Restrictions

The human maintainer exclusively controls all Git and GitHub operations.

NEVER:

- Execute Git commands.
- Execute GitHub CLI commands.
- Create, amend, revert, or modify commits.
- Push, pull, fetch, merge, rebase, stash, reset, or switch branches.
- Modify remotes, branches, tags, or repository settings.
- Create or modify pull requests or GitHub issues.

Do not use Git to inspect history, status, or diffs.

The maintainer runs every Git command manually.

## 3. Attribution Restrictions

NEVER add:

- Co-Authored-By: Codex
- Co-Authored-By: OpenAI
- Unwanted comments
- AI-generated commit attribution.
- AI attribution comments in source code.
- Unrequested AI credits in documentation.

Do not modify Git configuration or commit metadata.

## 4. File Safety

- Never delete or overwrite unrelated files.
- Never replace existing work without inspecting it first.
- Never modify files outside the authorized project scope.
- Never expose secrets, tokens, credentials, or private user data.
- Ask before destructive or irreversible changes.
- Explain proposed dependency additions before installing them.
- Do not run installation or environment-changing commands without approval.

## 5. Engineering Standards

- Use idiomatic, null-safe Dart.
- Follow official Flutter and Dart conventions.
- Prefer simple, modular, maintainable implementations.
- Avoid unnecessary abstractions and premature optimization.
- Keep features independently testable.
- Handle loading, empty, success, and error states.
- Include accessibility considerations.
- Respect both light and dark themes.
- Do not introduce unnecessary dependencies.
- Do not silently change established architecture or product decisions.

## 6. Product Principles

- Local-first and offline-first.
- No mandatory account or backend.
- User data remains private.
- No diagnostic or medical claims.
- Preserve historical workout and nutrition records.
- Provide reliable export, backup, and restoration.
- Never shame users for missed goals or inconsistent activity.

## 7. Testing and Quality

- Add tests for meaningful behavior.
- Run relevant analysis and tests when authorized.
- Never claim a test passed unless it actually ran successfully.
- Report failures and limitations honestly.
- Do not suppress analyzer warnings simply to obtain a clean result.

## 8. Working Procedure

Before substantial changes:

1. Inspect relevant existing files.
2. Explain the proposed approach.
3. Identify affected files.
4. Identify risks and dependencies.
5. Wait for authorization when the task requires it.

After changes:

1. Summarize implementation.
2. List created and modified files.
3. Report tests and analysis performed.
4. Report unresolved issues.
5. Suggest the next logical step.

## 9. Communication

- Be precise and concise.
- Explain important technical decisions.
- Do not invent requirements.
- Ask only essential clarification questions.
- Never assume permission to perform Git operations.

These instructions apply to all work performed by coding agents in this repository.
