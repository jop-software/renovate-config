<div align=center>
    <h1>jop-software/renovate-config</h1>
</div>

Shared renovate config for all projects.

## Usage

### From Github

```json5
// renovate.json
{
    "extends": [
        "github>jop-software/renovate-config"
    ]
}
```

### From npm

```json5
// renovate.json
{
    "extends": [
        "@jop-software"
    ]
}
```

See renovates docs about [Sharable Config Presets](https://docs.renovatebot.com/config-presets/) for more information.

## Features

### Auto Merging

This enables auto merging for all minor and patch updates as well as dev dependencies.

Automerging uses the `branch` strategy to not pollute the main branch with PRs.

### Package Rules

#### Github Artifacts Actions

Group all `actions/*-artifact` actions into one PullRequest, since they need to be updated together.

#### Automerge DEV Dependencies

Automerge all `devDependencies` updates.

#### Automerge Minor and Patch Updates

Automerge all minor and patch updates.

#### Grafana Loki

Groups `grafana/loki` and `grafana/promtail` together.

<div align=center>
    <span>&copy; 2024, jop-software Inh. Johannes Przymusinski</span>
</div>
    