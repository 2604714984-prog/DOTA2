# DOTA2 Scripts

A lightweight collection of Dota 2 scripts, automation tools, experiments, and utilities.

## Repository layout

Each tool lives in its own self-contained directory under `scripts/`:

```text
scripts/
  <script-name>/
```

Each script should keep its own README, dependencies, tests, changelog/version information, and runtime assets inside its directory.

## Scripts

| Script | Purpose | Current version |
| --- | --- | --- |
| [`boot-breaker-autoplayer`](scripts/boot-breaker-autoplayer/) | Boot Breaker minigame autoplayer and diagnostics tooling | v2.3.6 |

## Repository conventions

- Keep scripts independent unless shared code is genuinely useful across multiple tools.
- Do not commit local virtual environments, diagnostics, caches, temporary files, or machine-specific configuration.
- Put script-specific tests beside the script; repository-level CI may invoke those tests from `.github/workflows/`.
- Prefer small, readable changes and preserve working baselines before experimental control changes.

This repository is intended to remain a practical script collection rather than a large framework.
