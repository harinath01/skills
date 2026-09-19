# Skills Repository

This repository contains GitHub Copilot skills that should be installed with `skills.sh`.

## Required folder structure

`skills.sh` expects each skill to be in its own top-level directory. Keep the repository flat at the root level and place a `SKILL.md` file inside each skill directory. The `.installed-version` file is optional/used by the installer to track the installed version.

```text
skills/
├── basecamp/
│   ├── SKILL.md
│   └── .installed-version
├── create-branch/
│   ├── SKILL.md
│   └── .installed-version
├── documentation-writer/
│   ├── SKILL.md
│   └── .installed-version
├── grill-me/
│   ├── SKILL.md
│   └── .installed-version
├── improve-codebase-architecture/
│   ├── SKILL.md
│   └── .installed-version
├── tdd/
│   ├── SKILL.md
│   └── .installed-version
└── README.md
```

Important notes:

- Do not wrap skills in an extra `skills/` directory unless your `skills.sh` configuration specifically expects it.
- Each skill directory must contain a `SKILL.md` entry file.
- Keep the repository root focused on skill folders plus documentation.

## Installing with skills.sh

From the repository root, install using the `skills.sh` installer:

```bash
./skills.sh install .
```

If `skills.sh` is installed and available on your `PATH`, this is equivalent:

```bash
skills.sh install .
```

You can also point `skills.sh` at the repository directly:

```bash
skills.sh install https://github.com/harinath01/skills.git
```

This installs the skills into the location expected by `skills.sh` (for example, the configured agent skills directory such as `~/.agents/skills`).
