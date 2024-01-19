<div align=center>
    <h1>jop-software/renovate-config</h1>
</div>

Shared renovate config for all projects.

## Usage

```json5
// renovate.json
{
    "extends": [
        "github>jop-software/renovate-config"
    ]
}
```

## Features

### Package Rules

#### Github Artifacts Actions

Group all `actions/*-artifact` actions into one PullRequest, since they need to be updated together.

#### Automerge DEV Dependencies

Automerge all `devDependencies` updates.

#### Automerge Minor and Patch Updates

Automerge all minor and patch updates.

<div align=center>
    <span>&copy; 2024, jop-software Inh. Johannes Przymusinski</span>
</div>
    