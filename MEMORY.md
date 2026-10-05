# text-flags memory

Updated 2026-10-05. Version 1.0.1. Its own marketplace under the same name, installed as `text-flags@text-flags`.

## Layout

Single-plugin repo: plugin and marketplace at the root (`source: "./"`), marketplace named like the plugin, skill in `skills/`. CI runs `claude plugin validate --strict` and `npx skills add . --list` on every push.

## Release checklist

1. Bump `version` in `.claude-plugin/plugin.json`, or installed copies never update.
2. Add the changes to `CHANGELOG.md`.
3. Push, wait for the Validate workflow to pass, then tag `vX.Y.Z` and create a GitHub release.

## Decisions

- The plugin is named `text-flags` while its skill stays `text`, because a generic plugin name triggers a directory review hold and `/text` keeps working.
- `-l` absorbed the former timesheet skill: brief entries in the input's own voice, no consulting register.
- Every rule in `-p` traces to Anthropic's prompting docs, the best practices page and the Opus 5.5 and Sonnet 5.5 pages. Audited against them with live runs on 2026-10-05.
