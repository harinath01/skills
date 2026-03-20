# Skills Repository

This repository contains agent skills that can be synced to the `.agents` directory.

## Syncing Skills

To sync skills to the `.agents` directory:

```bash
rsync -av --ignore-existing --exclude='.git' --exclude='.gitignore' ./ ~/.agents/skills/
```

### Explanation

- `-a` - Archive mode (preserves permissions, timestamps, etc.)
- `-v` - Verbose output
- `--ignore-existing` - Skip files that already exist in destination
- `--exclude='.git'` - Exclude git directory
- `--exclude='.gitignore'` - Exclude gitignore file

### Alternative: Create a sync script

```bash
#!/bin/bash
rsync -av --ignore-existing --exclude='.git' --exclude='.gitignore' ./ ~/.agents/skills/
```

Save as `sync.sh` and run:

```bash
chmod +x sync.sh
./sync.sh
```
