# Gruntwork Marketplace

Claude Code plugins for Gruntwork development workflows.

## Installation

```bash
# Add marketplace (one time)
claude /plugin marketplace add gruntwork https://github.com/GruntworkAI/gruntwork-marketplace

# Install plugins
claude /plugin install lastmilefirst@gruntwork
```

## Available Plugins

| Plugin | Version | Description |
|--------|---------|-------------|
| [lastmilefirst](stack-wisdom/lastmilefirst/) | 0.3.0 | AI expert agents, CLAUDE.md management, project organization |

## About

This marketplace hosts plugins developed by [Gruntwork](https://github.com/GruntworkAI) for Claude Code. Each plugin follows the Last Mile First philosophy: set up the infrastructure for smooth delivery before building features.

## Architecture

Plugins are developed in [gruntwork-stack-wisdom](https://github.com/GruntworkAI/gruntwork-stack-wisdom) and included here via Git submodule. This means:
- Single source of truth for plugin code
- Updates to stack-wisdom automatically available when submodule is updated
- No code duplication or manual sync needed

To update to latest plugin versions:
```bash
git submodule update --remote
git commit -am "Update plugins to latest"
git push
```

## License

MIT
