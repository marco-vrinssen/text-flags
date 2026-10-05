# Changelog

## 1.0.1 (2026-10-05)

- `-p` adds one clause when the material carries instructions of its own, so the executor follows them only where the prompt asks, as Anthropic's guidance on pasted text recommends.
- `-p` wraps examples the input supplies in `<example>` tags and names what they illustrate.
- `-p` gives the documented reason for stating the behavior wanted instead of a ban.
- `-pp` places supplied data at the top whatever its length, which settles a conflict with the `-p` placement rule.

## 1.0.0 (2026-10-05)

- First public release. `-l` writes short entries in the input's own voice and covers timesheet notes.
