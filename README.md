# claude-plugins

A marketplace repository for Claude Code plugins.

## About

This repository contains plugins for [Claude Code](https://claude.ai/claude-code).
Each plugin is stored under the `plugins/` directory.

## Adding this marketplace

```
/plugin marketplace add tk0miya/claude-plugins
```

## Plugins

### init-ruby-project

Automates the initial setup of a Ruby project.

Sets up the following automatically:

- Scaffolding for a gem or a plain Ruby project
- RuboCop / Steep configuration files
- GitHub Actions workflows (test, Dependabot, auto-merge, release)
- VSCode settings
- GitHub repository creation and branch protection rules

#### Usage

```
/init-ruby-project
```
