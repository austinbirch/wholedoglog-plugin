# WholeDogLog for Claude

The WholeDogLog plugin, in a marketplace you can add from Claude's Customize > Plugins > Add marketplace.
The plugin itself is in [plugins/wholedoglog](./plugins/wholedoglog). [plugins/wholedoglog-staging](./plugins/wholedoglog-staging) is the staging build, for testing a branch.

## Versions

| Plugin | Channel | Version | Skill version |
| --- | --- | --- | --- |
| `wholedoglog` | production | 0.1.143 | `b7060564` |
| `wholedoglog-staging` | staging | 0.0.544 | `532dc2c9` |

Production's version is `0.1.` and the number of commits that changed the skill; staging's is `0.0.` and the run of the Staging workflow that published it, so the two never match. The skill version is on the first line of each skill's SKILL.md (and in its `metadata.version`), which a chat sends back as `skillVersion`.

This repository is generated from WholeDogLog's own; changes made here are overwritten.
