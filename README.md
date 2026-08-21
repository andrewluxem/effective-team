# effective-team

Builds an evidence-bound team health check and action plan without judging personalities.

It produces:

- **Team Health Check and Action Plan:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Effective Team playbook](https://www.andrewluxem.com/playbooks/effective-team). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/effective-team.git
cp -r effective-team/skills/effective-team ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r effective-team/skills/effective-team ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/effective-team
/plugin install effective-team@effective-team
```

For clients that install from an archive, use the versioned [effective-team v1.0.0 ZIP](https://www.andrewluxem.com/downloads/effective-team-v1.0.0.zip).

## Invoke it

```text
Run a team health check and action plan
Use the effective-team skill.
```

Naming the skill is always valid: `use the effective-team skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/effective-team/
  assets/team-health-check-template.md
  LICENSE.md
  meta.yaml
  references/team-health-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/effective-team/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/effective-team/LICENSE.md](skills/effective-team/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.