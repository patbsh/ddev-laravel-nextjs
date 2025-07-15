# DDEV Laravel + Next.js Addon

A DDEV addon that sets up a Laravel backend with Next.js frontend in separate containers.

## What it does

- Creates a fresh Laravel project in `/backend` directory
- Creates a fresh Next.js project in `/frontend` directory  
- Configures environment files for both
- Sets up proper routing:
  - Frontend: `https://projectname.ddev.site`
  - Backend API: `https://api.projectname.ddev.site`

## Installation

```bash
ddev get /path/to/this/addon
```

## Usage

After installation, bootstrap your project:

```bash
ddev laravel-nextjs-setup
```

## Available Commands

- `ddev artisan` - Run Laravel artisan commands
- `ddev npm-frontend` - Run npm commands in frontend directory
- `ddev laravel-nextjs-setup [--force]` - Bootstrap the project (use --force to overwrite existing)

## Project Structure

```
project/
├── backend/          # Laravel application
├── frontend/         # Next.js application
└── .ddev/           # DDEV configuration
```

## Next Steps

1. Run `ddev artisan migrate` to set up your database
2. Start building your application!

## URLs

- Frontend: `https://projectname.ddev.site`
- Backend: `https://api.projectname.ddev.site`
- Database: Available to both containers as `db` host
