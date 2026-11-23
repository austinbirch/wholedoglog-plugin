# WholeDogLog for Claude

The WholeDogLog plugin, in a marketplace you can add from Claude's Customize > Plugins > Add marketplace.
The plugin itself is in [plugins/wholedoglog](./plugins/wholedoglog). [plugins/wholedoglog-staging](./plugins/wholedoglog-staging) is the staging build, for testing a branch.

## Versions

| Plugin | Channel | Version | Skill version |
| --- | --- | --- | --- |
| `wholedoglog` | production | 0.1.137 | `45ca318f` |
| `wholedoglog-staging` | staging | 0.0.533 | `d458ec9b` |

Production's version is `0.1.` and the number of commits that changed the skill; staging's is `0.0.` and the run of the Staging workflow that published it, so the two never match. The skill version is the `metadata.version` in each skill's SKILL.md, which a chat sends back as `skillVersion`.

This repository is generated from WholeDogLog's own; changes made here are overwritten.
