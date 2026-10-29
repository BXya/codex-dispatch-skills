# Source

## Attribution

The included skill comes from [obra/superpowers](https://github.com/obra/superpowers), specifically `skills/dispatching-parallel-agents/SKILL.md`, by Jesse Vincent, under the MIT license. The license text, including the line `Copyright (c) 2025 Jesse Vincent`, is kept in this repository and in the installable skill folder.

This is an independent redistribution. It does not claim original authorship, upstream endorsement, or any official OpenAI affiliation.

## Upstream version

With LF line endings, `skills/dispatching-parallel-agents/SKILL.md` matches the upstream file byte for byte at commit [`f0e5117fa6bdd2645485d2a8df8d7a107c4bf2af`](https://github.com/obra/superpowers/commit/f0e5117fa6bdd2645485d2a8df8d7a107c4bf2af) ("Phase A: agent-neutral prose + CSO → SDO + spec", 2026-06-16). Its LF Git blob hash is `75e7e22cef2e7adc0963e74457cf2664514dee33`.

This identifies the upstream version used in the v6.0.0–v6.1.1 release range. The release tags checked directly were [v6.0.0](https://github.com/obra/superpowers/blob/v6.0.0/skills/dispatching-parallel-agents/SKILL.md), [v6.0.3](https://github.com/obra/superpowers/blob/v6.0.3/skills/dispatching-parallel-agents/SKILL.md), and [v6.1.1](https://github.com/obra/superpowers/blob/v6.1.1/skills/dispatching-parallel-agents/SKILL.md); all three contain the same blob.

The skill file was published without changes. Git checkout settings can produce CRLF line endings; the LF identity above distinguishes content provenance from checkout bytes.

Upstream revised the skill starting with v6.2.0. Commit [`6dbbbda3baeff8407f3dddb0cc9e8a9495a273bc`](https://github.com/obra/superpowers/commit/6dbbbda3baeff8407f3dddb0cc9e8a9495a273bc) removed the "Key Benefits" and "Real-World Impact" sections. For the current version, use obra/superpowers directly.

## Correction (2026-10-29)

An earlier version of this note called the file a local adaptation and said it differed from the plugin copy only in section 3, "Dispatch in Parallel". That description was wrong:

- The plugin copy used for the comparison had older 5.1.x metadata. The upstream v5.1.0 file also uses the older `Task(...)` examples. Comparing against that older copy did not establish a local adaptation.
- The section 3 wording comes from upstream commit `f0e5117fa6bdd2645485d2a8df8d7a107c4bf2af`, not from a local edit. It includes the `Subagent (general-purpose)` example and guidance to issue several dispatches in the same response.

## Limits

Runtime compatibility and the concurrency claim have not been checked in practice. File and release comparisons establish content identity, not behavioral compatibility. The old plugin's precise upstream commit was not established from its local version metadata.

## Fingerprints

Hashes are of the files as committed to this repository. `SKILL.md` is committed with LF line endings; both `LICENSE` copies are committed with CRLF line endings. A checkout with `core.autocrlf` enabled will show different bytes on disk.

| File (as committed) | SHA256 | Git blob |
| --- | --- | --- |
| `skills/dispatching-parallel-agents/SKILL.md` (LF) | `f0df13f584049059cc5619f90061405b89dcc6e28ab3f2a8517d27d99c7a46a6` | `75e7e22cef2e7adc0963e74457cf2664514dee33` |
| `LICENSE` and `skills/dispatching-parallel-agents/LICENSE` (CRLF) | `0da33ed814ee87e72db078f489c4447af72f13d9f25d9e17476f32efd77705fc` | `5389576ae59896f16bba7391ceebdfb6f29a8584` |
