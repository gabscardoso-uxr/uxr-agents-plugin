# uxr-agents

A Claude Code plugin with UX Research skills that transform briefs into decision-ready research artifacts.

## Skills

| Skill | Command | What it does |
|---|---|---|
| **Scoper** | `/uxr-agents:scoper` | Transforms vague briefs into decision-ready research plans with stage-aware gating |
| **Screener** | `/uxr-agents:screener` | Generates field-ready participant screeners from a research scope |
| **Discussion Guide** | `/uxr-agents:discussion-guide` | Generates field-ready discussion guides from a research scope |
| **Synthesis** | `/uxr-agents:synthesis` | Transforms raw session notes into structured decision-ready findings |

## Installation

1. Add the marketplace:

   ```
   /plugin marketplace add gabscardoso-uxr/uxr-agents-plugin
   ```

2. Install the plugin:

   ```
   /plugin install uxr-agents@uxr-agents
   ```

3. Reload plugins:

   ```
   /reload-plugins
   ```

## Usage

Start with scoping a research brief:

```
/uxr-agents:scoper
```

Then paste your brief. Scoper will first output a pre-flight checklist (stage, evidence, downstream gates) and stop. Confirm or correct the stage in a new turn — only then will it produce the full scope.

Once you have a scope, generate supporting artifacts:

```
/uxr-agents:screener
/uxr-agents:discussion-guide
```

After fieldwork, synthesize your findings:

```
/uxr-agents:synthesis
```

## Contributing

The canonical source for these skills is [gabscardoso-uxr/uxr-agents](https://github.com/gabscardoso-uxr/uxr-agents). This repo is a read-only distribution — file issues and PRs against the source repo.

## License

MIT
