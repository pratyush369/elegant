# My Theme Fork - Build Instructions

This is a local fork of the [Pelican-Elegant](https://github.com/Pelican-Elegant/elegant) theme with custom modifications.

## Local Development Setup

### Prerequisites
- Node.js (for npm/yarn)
- Python virtual environment with invoke installed

### Build Theme Assets

```bash
# Build theme CSS and JS
yarn build

# Or with npm
npm run build

# Watch mode with live reload
yarn dev
```

### Repository Structure

- `static/` - Theme assets (CSS, JS, fonts)
- `templates/` - Jinja2 HTML templates
- `gulpfile.babel.js` - Build configuration (theme compilation)
- `package.json` - Node.js dependencies and scripts

## Git Workflow

### Update from Upstream

```bash
# Fetch latest changes from main elegant repo
git fetch upstream

# Merge or rebase with upstream master
git rebase upstream/master

# Push to your fork
git push origin master
```

### Push Local Changes

```bash
# Stage changes
git add .

# Commit
git commit -m "Description of changes"

# Push to your fork
git push origin master
```

## Available Commands

| Command | Purpose |
|---------|---------|
| `yarn build` | Compile theme assets (CSS/JS) |
| `yarn dev` | Watch mode with browser sync |
| `yarn build:docs` | Build full documentation site |
| `yarn validate` | Validate Jinja2 templates |

## Notes

- Build outputs go to `static/css/` and `static/js/`
- The theme is designed for Pelican static site generator
- Always test changes locally before pushing
- Keep fork synchronized with upstream main repository

## References

- [Elegant Theme GitHub](https://github.com/Pelican-Elegant/elegant)
- [Pelican Documentation](https://docs.getpelican.com/)
