[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/OpenForgeProject/ddev-skills/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/OpenForgeProject/ddev-skills/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/OpenForgeProject/ddev-skills)](https://github.com/OpenForgeProject/ddev-skills/commits)
[![release](https://img.shields.io/github/v/release/OpenForgeProject/ddev-skills)](https://github.com/OpenForgeProject/ddev-skills/releases/latest)

# DDEV Skills

## Overview

This add-on integrates Skills into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get OpenForgeProject/ddev-skills
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Skills |
| `ddev logs -s skills` | Check Skills logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.skills --skills-docker-image="ddev/ddev-utilities:latest"
ddev add-on get OpenForgeProject/ddev-skills
ddev restart
```

Make sure to commit the `.ddev/.env.skills` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `SKILLS_DOCKER_IMAGE` | `--skills-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@OpenForgeProject](https://github.com/OpenForgeProject)**
