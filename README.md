# Skills Repository

This repository contains agent skills installable with [skills.sh](https://skills.sh/).

## Installation

Install this repository with the official skills.sh installer:

```bash
npx skills@latest add harinath01/skills
```

You can also install a specific skill from the repo:

```bash
npx skills@latest add harinath01/skills --skill <skill-name>
```

## Repository structure

This repository follows the layout expected by skills.sh. Each skill is stored in its own top-level directory, and each directory contains a `SKILL.md` file:

```text
skills/
├── basecamp/
│   └── SKILL.md
├── commit/
│   └── SKILL.md
├── create-branch/
│   └── SKILL.md
├── documentation-writer/
│   └── SKILL.md
├── grill-me/
│   └── SKILL.md
├── improve-codebase-architecture/
│   └── SKILL.md
├── tdd/
│   └── SKILL.md
└── README.md
```

Important notes:

- Each skill directory is a top-level folder in the repo root.
- Each folder contains a `SKILL.md` file.
- The directory name should match the skill name used by the installer.
- This repo does not use an extra nested `skills/` directory wrapper.

## Available skills

- `basecamp`
- `commit`
- `create-branch`
- `documentation-writer`
- `grill-me`
- `improve-codebase-architecture`
- `tdd`

For more details, see the official docs at [skills.sh](https://skills.sh/).
