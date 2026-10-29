# Codex Dispatch Skills

An unmodified upstream copy of Superpowers' `dispatching-parallel-agents` skill from v6.0.0–v6.1.1 for coordinating independent tasks with subagents.

This is an independent redistribution, not an official OpenAI or Superpowers release. See [SOURCE.md](SOURCE.md) for provenance and upstream version details.

Upstream revised this skill in v6.2.0 and later; use [obra/superpowers](https://github.com/obra/superpowers) directly for the latest version.

## Included skill

| Skill | Purpose |
| --- | --- |
| [dispatching-parallel-agents](skills/dispatching-parallel-agents/SKILL.md) | Divide independent work into focused tasks, dispatch subagents, and review their results. |

Only this confirmed skill is included. It has no bundled executable scripts, package dependencies, external services, or credentials.

## Install

Clone this repository or download its ZIP. Copy the entire `skills/dispatching-parallel-agents` folder, including its `LICENSE`, into the skills directory used by your Codex installation.

For installations using `$CODEX_HOME/skills`, or `~/.codex/skills` when `CODEX_HOME` is unset, run one of the following from this repository's root. These commands stop if a skill with the same name is already installed.

PowerShell:

```powershell
$ErrorActionPreference = 'Stop'
$codexRoot = if ($env:CODEX_HOME) { $env:CODEX_HOME } else { Join-Path $env:USERPROFILE '.codex' }
$skillsRoot = Join-Path $codexRoot 'skills'
$destination = Join-Path $skillsRoot 'dispatching-parallel-agents'
if (Test-Path -LiteralPath $destination) { throw 'Skill already exists; review it before replacing it.' }
New-Item -ItemType Directory -Path $skillsRoot -Force | Out-Null
Copy-Item -LiteralPath './skills/dispatching-parallel-agents' -Destination $destination -Recurse
```

Bash:

```bash
skills_root="${CODEX_HOME:-$HOME/.codex}/skills"
destination="$skills_root/dispatching-parallel-agents"
if [ -e "$destination" ] || [ -L "$destination" ]; then
  printf '%s\n' 'Skill already exists; review it before replacing it.' >&2
else
  mkdir -p "$skills_root" && cp -R ./skills/dispatching-parallel-agents "$destination"
fi
```

Start a new Codex session and invoke `$dispatching-parallel-agents` with a task that contains independent work. If your setup uses a different skills directory, use that directory instead.

## Compatibility and validation

- The host assistant must provide subagent tools. The skill does not add those tools.
- `Subagent (general-purpose)` in the examples is illustrative text, not a portable API. Tool names, dispatch grouping, and actual concurrency depend on the host runtime.
- The upstream content is unmodified. In particular, the statement about dispatching in one response should not be treated as a runtime guarantee.
- Historical test outcomes in the skill are upstream examples, not test results for this distribution. Packaging and static checks do not establish end-to-end subagent behavior.

## License

The original [MIT license](LICENSE), including the copyright notice for Jesse Vincent, is retained. A copy is included inside the skill folder so it remains present when that folder is installed or redistributed separately.
