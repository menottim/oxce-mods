# OXCE Mods Collection

## Overview

A collection of OXCE mods published to github.com/menottim/oxce-mods. Each mod is a folder with `metadata.yml` + `.rul` files.

## Git Identity

Always use personal identity:
```
git -c user.name="menottim" -c user.email="menottim@users.noreply.github.com" commit ...
```

## Validation

Validate any mod folder with the oxce-modgen validator:
```bash
python3 ~/oxce-modgen/scripts/validate_mod.py <mod-folder>
```

## Documentation Maintenance (MUST FOLLOW)

When adding or modifying mods, you MUST update documentation in the same commit:

| Change type | Documents to update |
|-------------|-------------------|
| New mod added | README.md — add entry under "Mods" section with description, pricing/stats table, folder link |
| Mod updated | README.md — update the mod's description and stats if they changed |
| Mod removed | README.md — remove the entry |
| Any README section change | README.md "Table of Contents" — update links to match |

__README.md__ is the public-facing catalog. Every mod must have a section there with a description, key stats, and a link to its folder.

## Adding a New Mod

1. Create `<mod-name>/metadata.yml` with required fields (name, version, description, author, master)
2. Create `<mod-name>/<mod-name>.rul` with YAML overrides
3. Validate: `python3 ~/oxce-modgen/scripts/validate_mod.py <mod-name>/`
4. Add a section to README.md under "Mods" (update ToC too)
5. Commit and push
