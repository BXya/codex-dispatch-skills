# Source and local adaptation

## Attribution

The included skill is derived from [obra/superpowers](https://github.com/obra/superpowers), specifically `skills/dispatching-parallel-agents/SKILL.md`.

The locally available Superpowers plugin metadata identifies Jesse Vincent as its author, declares version `5.1.3`, and points to that repository under the MIT license. The accompanying license states `Copyright (c) 2025 Jesse Vincent`; its complete text is preserved in this repository and in the installable skill folder.

This is an independent redistribution of a locally installed adaptation. It does not claim original authorship, upstream endorsement, or official OpenAI affiliation.

## What was preserved

`skills/dispatching-parallel-agents/SKILL.md` is copied byte for byte from the local standalone skill. No instruction changes were made for this publication.

Compared with the locally available plugin copy, the only text difference after normalizing line endings is in **3. Dispatch in Parallel**:

- The plugin copy uses a TypeScript code block with Claude Code-style `Task(...)` calls.
- The standalone adaptation uses a text block with `Subagent (general-purpose)` examples and adds guidance about issuing multiple dispatches in the same response.
- The standalone file uses LF line endings; the plugin file uses CRLF.

The package includes the standalone adaptation only. The plugin's optional `agents/openai.yaml` UI metadata is not mixed into it.

## Provenance limits

The upstream Git commit corresponding to the locally available plugin was not verified. Its version metadata is provenance evidence, not a release version assigned to this adaptation. The identity and date of the local modification were not established. Runtime compatibility and the concurrency claim have not been behaviorally verified.

The README and this source note were added for packaging. The skill and original license were preserved without changes.

## SHA256 fingerprints

| Material | SHA256 |
| --- | --- |
| Published standalone `SKILL.md` | `f0df13f584049059cc5619f90061405b89dcc6e28ab3f2a8517d27d99c7a46a6` |
| Comparison plugin `SKILL.md` (not included) | `ee429867974830f3fa1dc2a3b0cf5c98c742a1c33ec0fb156ac3727a255d24b5` |
| Original MIT `LICENSE` (both included copies) | `0da33ed814ee87e72db078f489c4447af72f13d9f25d9e17476f32efd77705fc` |
