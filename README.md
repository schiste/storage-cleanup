# Storage Cleanup

An Agent Skill for investigating and reclaiming disk space while distinguishing rebuildable artifacts from personal data and active work.

**Current platform coverage: macOS.** The project name allows other operating systems to be added later; it does not imply that Linux or Windows cleanup procedures are already supported. The skill needs an agent with appropriate access to the target computer, or it can provide instructions for a person to run.

## Install and use

Clone `https://github.com/schiste/storage-cleanup.git` or download this repository, then install or link its directory as `storage-cleanup` in the skills directory used by your agent. Keep `SKILL.md` and `references/` together. Consult your agent's documentation for its installation location and invocation syntax. For example, a Codex user can link the checkout into `~/.codex/skills/storage-cleanup` and invoke `$storage-cleanup`. `agents/openai.yaml` is optional metadata for compatible OpenAI environments; other agents need only the skill and its referenced files.

Ask the agent to audit storage, or explicitly authorize the categories you want cleaned. An audit alone does not authorize deletion. Review reported limitations and recovery risks, especially for backups, synchronized files, development projects, and agent histories.

## Contribute

[Issues](https://github.com/schiste/storage-cleanup/issues) and pull requests are welcome from everyone, including people without maintainer permissions. See [CONTRIBUTING.md](CONTRIBUTING.md). Describe reproducible improvements without sharing private machine data. The skill can help draft an issue when a user permits external posting.

## License

[MIT](LICENSE).
