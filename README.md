# Skills

A collection of skills for AI agents. Each skill provides instructions for a specific type of task and can be installed separately.

[![Agent Skills](https://img.shields.io/badge/format-Agent_Skills-2563eb)](https://agentskills.io)
![Markdown](https://img.shields.io/badge/instructions-Markdown-222222)
[![Node.js](https://img.shields.io/badge/Node.js-%3E%3D22.20-339933)](https://github.com/vercel-labs/skills/blob/main/package.json)
[![MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)

Instructions are written in Markdown using the Agent Skills format. The [skills CLI](https://github.com/vercel-labs/skills) handles installation and updates.

## Catalog

Browse the [catalog](skills/README.md) for available skills and short descriptions. Each skill's `SKILL.md` contains its full instructions and scope.

## Requirements

- Node.js 22.20 or later and npm with `npx`.
- Git to download the repository.
- An agent that supports Agent Skills. See the [supported agents](https://github.com/vercel-labs/skills/blob/main/docs/agents.md).

Installation requires access to npm and GitHub. The Node.js requirement applies to the CLI; any additional requirements are listed in each skill's instructions.

## Installation

Install skills from this repository:

```bash
npx skills@latest add stobartt/skills
```

Follow the CLI prompts to select skills and an agent. Skills are installed in the current project by default. Add `--global` to make them available across projects.

List available skills without installing them:

```bash
npx skills@latest add stobartt/skills --list
```

## Usage

Describe your task and provide the relevant source material. Agents that support automatic skill selection can choose a matching skill based on your request.

To select a skill explicitly, mention its name in your request or use your agent's skill command or menu. The exact method depends on the agent. See each skill's `SKILL.md` for its purpose and instructions.

## Updates

Update installed skills:

```bash
npx skills@latest update
```

The CLI prompts you to select an installation scope. Use `--global` or `--project` to select it explicitly. This command updates skills in that scope, including those from other repositories. To update a single skill, add its name after `update`.

GitHub updates are tracked after installation through `skills add`. Files copied into an agent's skill directory manually are not automatically linked to their repository. When switching to the CLI, keep one installed copy of each skill. See the [CLI reference](https://github.com/vercel-labs/skills/blob/main/docs/commands.md) for command options.

## Distribution

Skills are installed from the public [stobartt/skills](https://github.com/stobartt/skills) repository. The CLI downloads published files from the default branch. Changes become available after they are pushed to that branch; users receive them through the update command.

GitHub is sufficient for distribution. A separate npm package or file upload to skills.sh is not required. According to the [skills.sh FAQ](https://skills.sh/docs/faq), the directory tracks skills automatically through CLI installation telemetry. A directory listing is not required to install from the repository.

Check skill discovery in a local checkout:

```bash
npx skills@latest add . --list
```

## License

[MIT](LICENSE). Attribution and applicable terms for source material are retained in the skill files.
