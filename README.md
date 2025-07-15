[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/patbsh/ddev-laravel-nextjs/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/patbsh/ddev-laravel-nextjs/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/patbsh/ddev-laravel-nextjs)](https://github.com/patbsh/ddev-laravel-nextjs/commits)
[![release](https://img.shields.io/github/v/release/patbsh/ddev-laravel-nextjs)](https://github.com/patbsh/ddev-laravel-nextjs/releases/latest)

# DDEV Laravel Nextjs

## Overview

This add-on integrates Laravel Nextjs into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get patbsh/ddev-laravel-nextjs
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Laravel Nextjs |
| `ddev logs -s laravel-nextjs` | Check Laravel Nextjs logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.laravel-nextjs --laravel-nextjs-docker-image="busybox:stable"
ddev add-on get patbsh/ddev-laravel-nextjs
ddev restart
```

Make sure to commit the `.ddev/.env.laravel-nextjs` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `LARAVEL_NEXTJS_DOCKER_IMAGE` | `--laravel-nextjs-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@patbsh](https://github.com/patbsh)**
