# Super Simple Marketplace

A Claude Cowork / Claude Code marketplace registry that distributes the **super-simple** plugin.

## Structure

```
super-simple-marketplace/
├── .claude-plugin/
│   └── marketplace.json      # Marketplace registry
├── super-simple/              # Plugin (git submodule or copy)
│   ├── .claude-plugin/
│   │   └── plugin.json
│   └── skills/
│       └── write-prd/
│           ├── SKILL.md
│           └── references/
│               └── product-brief-template.md
└── README.md
```

## Setup

The marketplace expects the plugin to be available at `./super-simple/`. You can either:

1. **Git submodule** (recommended):
   ```bash
   git submodule add <super-simple-plugin-repo-url> super-simple
   ```

2. **Copy** the `super-simple-plugin` repo contents into the `super-simple/` directory.
