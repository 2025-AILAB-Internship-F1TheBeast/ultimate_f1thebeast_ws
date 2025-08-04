# Ultimate F1TheBeast Team Repository

## Setup

### Clone with submodules
```bash
git clone --recurse-submodules https://github.com/2025-AILAB-Internship-F1TheBeast/ultimate_f1thebeast_ws.git
```

### If already cloned
```bash
git submodule update --init --recursive
```

## Daily Usage

### Get latest updates
```bash
git pull --recurse-submodules
```

### Make changes in main repo
```bash
git add .
git commit -m "Your message"
git push
```

### Make changes in submodule
```bash
# Work in submodule
cd submodule_folder
git add .
git commit -m "Update submodule"
git push

# Update main repo reference
cd ..
git add submodule_folder
git commit -m "Update submodule reference"
git push
```

### Update all submodules to latest
```bash
git submodule update --remote --recursive
git add .
git commit -m "Update submodules"
git push
```

## Troubleshooting

### Missing submodule content
```bash
git submodule update --init --recursive --force
```

### Check submodule status
```bash
git submodule status --recursive
```

## Key Points
- Always use `--recursive` flag for nested submodules
- Commit changes in submodule first, then update main repo reference
- Use `git pull --recurse-submodules` to get all updates
